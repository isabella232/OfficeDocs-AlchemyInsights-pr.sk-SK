---
title: Riešenie problému s PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573907"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="c430b-102">Riešenie problému s PRT</span><span class="sxs-lookup"><span data-stu-id="c430b-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="c430b-103">Ak chcete, aby všetky zariadenia dokončili overenie, musí byť plne zaregistrovaný a v dobrom stave a môže získať primárny token obnovenia (PRT).</span><span class="sxs-lookup"><span data-stu-id="c430b-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="c430b-104">Proces registrácie hybridnej Azure AD sa vyžaduje, aby sa zariadenia nachádzali v podnikovej sieti.</span><span class="sxs-lookup"><span data-stu-id="c430b-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="c430b-105">Funguje aj cez VPN, ale tam sú niektoré námietky na to.</span><span class="sxs-lookup"><span data-stu-id="c430b-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="c430b-106">Počuli sme zákazníkov, ktorí potrebujú pomoc pri riešení problémov s procesom registrácie hybridnej služby Azure AD v rámci podmienok vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="c430b-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="c430b-107">Tu je rozpis toho, čo sa deje pod kapotou počas procesu registrácie.</span><span class="sxs-lookup"><span data-stu-id="c430b-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="c430b-108">**Cloudové overovanie prostredia (pomocou synchronizácie hash hesla služby Azure AD alebo overovacieho overovania)**</span><span class="sxs-lookup"><span data-stu-id="c430b-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="c430b-109">Tento registračný tok sa označuje aj ako synchronizačný spoj.</span><span class="sxs-lookup"><span data-stu-id="c430b-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="c430b-110">Windows 10 zistí záznam SCP pri prihlásení používateľa do zariadenia.</span><span class="sxs-lookup"><span data-stu-id="c430b-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="c430b-111">Zariadenie sa najprv pokúsi o načítanie informácií o nájomníkovi z SCP na strane klienta v databáze Registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="c430b-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="c430b-112">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="c430b-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="c430b-113">Ak to zlyhá, zariadenie komunikuje s lokálnou službou Active Directory (AD) na získanie informácií o nájomníkovi z bodu pripojenia služby (SCP).</span><span class="sxs-lookup"><span data-stu-id="c430b-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="c430b-114">Ak chcete overiť SCP, prečítajte si tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="c430b-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="c430b-115">Odporúčame povoliť SCP v REKLAMe a len na strane klienta SCP na prvotné overenie.</span><span class="sxs-lookup"><span data-stu-id="c430b-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="c430b-116">Windows 10 sa pokúša komunikovať so službou Azure AD v rámci systémového kontextu, aby sa overil sám proti službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c430b-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="c430b-117">Ak chcete overiť, či zariadenie môže získať prístup k prostriedkom spoločnosti Microsoft v rámci systémového konta, pomocou skriptu na pripojenie k registrácii testovacieho zariadenia.</span><span class="sxs-lookup"><span data-stu-id="c430b-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="c430b-118">Windows 10 generuje certifikát s vlastným podpisom a uloží ho pod objekt počítača v lokálnej REKLAMe.</span><span class="sxs-lookup"><span data-stu-id="c430b-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="c430b-119">Tento postup vyžaduje, aby sa na radiči domény začiarkli.</span><span class="sxs-lookup"><span data-stu-id="c430b-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="c430b-120">Objekt zariadenia s certifikátom sa synchronizuje so službou Azure AD prostredníctvom služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c430b-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="c430b-121">Cyklus synchronizácie je predvolene každých 30 minút, ale závisí to od konfigurácie služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c430b-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="c430b-122">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="c430b-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="c430b-123">V tejto fáze by ste mali mať možnosť Zobraziť predmetové zariadenie v stave čaká sa v časti čepeľ zariadenia na portáli Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="c430b-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="c430b-124">Pri ďalšom prihlásení používateľa do Windowsu 10 sa registrácia ukončí.</span><span class="sxs-lookup"><span data-stu-id="c430b-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="c430b-125">Ak sa nachádzate na sieti VPN a proces prihlásenia odhlásenie ukončí pripojenie k doméne, môžete spustiť registráciu manuálne:</span><span class="sxs-lookup"><span data-stu-id="c430b-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="c430b-126">Vydať dsregcmd/JOIN lokálne na výzvu správcu alebo vzdialene cez PSExec do počítača.</span><span class="sxs-lookup"><span data-stu-id="c430b-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="c430b-127">Napríklad PsExec-s \\ win10client01 cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="c430b-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="c430b-128">Ďalšie informácie o problémoch s hybridným spojením nájdete v téme [Riešenie problémov s zariadeniami](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="c430b-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
