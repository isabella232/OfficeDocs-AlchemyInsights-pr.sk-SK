---
title: Zariadenie v stave čakajúce
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679991"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="1d079-102">Zariadenie v stave čakajúce</span><span class="sxs-lookup"><span data-stu-id="1d079-102">Device in pending state</span></span>

<span data-ttu-id="1d079-103">**Predpoklady**</span><span class="sxs-lookup"><span data-stu-id="1d079-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="1d079-104">Ak nastavujete registráciu zariadenia prvýkrát, skontrolujte, či ste si prezreli [úvodné informácie o správe zariadení v službe Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , ktorá vám poskytne informácie o tom, ako získať zariadenia pod kontrolou služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1d079-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="1d079-105">Ak registrujete zariadenia do služby Azure AD priamo a prihlásite ich do služby Intune, budete musieť zabezpečiť [konfiguráciu služby Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a mať [licenciu](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) na mieste ako prvý.</span><span class="sxs-lookup"><span data-stu-id="1d079-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="1d079-106">Uistite sa, že máte oprávnenie vykonávať operácie v službe Azure AD a lokálnu reklamu.</span><span class="sxs-lookup"><span data-stu-id="1d079-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="1d079-107">Nastavenie registrácií zariadenia môže spravovať len globálny správca v službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1d079-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="1d079-108">Okrem toho, Ak nastavujete automatické registrácie v lokálnej službe Active Directory, budete musieť byť správcom služby Active Directory a AD FS (ak je to možné).</span><span class="sxs-lookup"><span data-stu-id="1d079-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="1d079-109">Proces registrácie hybridnej Azure AD sa vyžaduje, aby sa zariadenia nachádzali v podnikovej sieti.</span><span class="sxs-lookup"><span data-stu-id="1d079-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="1d079-110">Funguje aj cez VPN, ale tam sú niektoré námietky na to.</span><span class="sxs-lookup"><span data-stu-id="1d079-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="1d079-111">Počuli sme zákazníkov, ktorí potrebujú pomoc pri riešení problémov s procesom registrácie hybridnej služby Azure AD v rámci vzdialenej pracovnej situácie.</span><span class="sxs-lookup"><span data-stu-id="1d079-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="1d079-112">**Cloudové overovanie prostredia (pomocou synchronizácie hash hesla služby Azure AD alebo overovacieho overovania)**</span><span class="sxs-lookup"><span data-stu-id="1d079-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="1d079-113">Tento registračný tok sa označuje aj ako synchronizačný spoj.</span><span class="sxs-lookup"><span data-stu-id="1d079-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="1d079-114">Tu je rozpis toho, čo sa deje počas procesu registrácie:</span><span class="sxs-lookup"><span data-stu-id="1d079-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="1d079-115">Windows 10 zistí záznam bodu pripojenia služby (SCP), keď sa používateľ prihlási do zariadenia.</span><span class="sxs-lookup"><span data-stu-id="1d079-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="1d079-116">Zariadenie sa najprv pokúsi o načítanie informácií o nájomníkovi z SCP na strane klienta v databáze Registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="1d079-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="1d079-117">Ďalšie informácie nájdete v téme [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="1d079-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="1d079-118">Ak sa to nepodarí, zariadenie komunikuje s lokálnou službou Active Directory na získanie informácií o nájomníkovi z SCP.</span><span class="sxs-lookup"><span data-stu-id="1d079-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="1d079-119">Ak chcete overiť SCP, prečítajte si tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="1d079-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="1d079-120">Odporúčame povoliť SCP v službe Active Directory a použiť len SCP na strane klienta na prvotné overenie.</span><span class="sxs-lookup"><span data-stu-id="1d079-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="1d079-121">Windows 10 sa pokúša komunikovať so službou Azure AD v rámci systémového kontextu, aby sa overil sám proti službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1d079-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="1d079-122">Ak chcete overiť, či zariadenie môže získať prístup k prostriedkom spoločnosti Microsoft v rámci systémového konta, pomocou [skriptu na pripojenie k registrácii testovacieho zariadenia](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="1d079-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="1d079-123">Windows 10 generuje certifikát s vlastným podpisom a uloží ho pod objekt počítača v lokálnej službe Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1d079-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="1d079-124">Tento postup vyžaduje, aby sa na radiči domény začiarkli.</span><span class="sxs-lookup"><span data-stu-id="1d079-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="1d079-125">Objekt zariadenia s certifikátom sa synchronizuje so službou Azure AD prostredníctvom služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1d079-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="1d079-126">Cyklus synchronizácie je predvolene každých 30 minút, ale závisí to od konfigurácie služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1d079-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="1d079-127">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="1d079-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="1d079-128">V tejto fáze by ste mali mať možnosť Zobraziť predmetové zariadenie v stave **čaká** sa v časti čepeľ zariadenia na portáli Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1d079-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="1d079-129">Pri ďalšom prihlásení používateľa do Windowsu 10 sa registrácia ukončí.</span><span class="sxs-lookup"><span data-stu-id="1d079-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1d079-130">Ak sa nachádzate na virtuálnej súkromnej sieti a odhlásenie/prihlásenie ukončí pripojenie k doméne, môžete spustiť registráciu manuálne.</span><span class="sxs-lookup"><span data-stu-id="1d079-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="1d079-131">Ak to chcete urobiť, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="1d079-131">To do that:</span></span>
    >
    > <span data-ttu-id="1d079-132">Vydá `dsregcmd /join` lokálne na výzvu správcu alebo na diaľku cez PSExec do počítača.</span><span class="sxs-lookup"><span data-stu-id="1d079-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="1d079-133">Príklad: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="1d079-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="1d079-134">Bežné problémy s registráciou zariadenia služby Azure Active Directory nájdete v téme [najčastejšie otázky o zariadeniach](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="1d079-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
