---
title: Synchronizácia hesla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483083"
---
# <a name="password-synchronization"></a><span data-ttu-id="faf1e-102">Synchronizácia hesla</span><span class="sxs-lookup"><span data-stu-id="faf1e-102">Password synchronization</span></span>

<span data-ttu-id="faf1e-103">**Synchronizácia hash hesla nefunguje vôbec**</span><span class="sxs-lookup"><span data-stu-id="faf1e-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="faf1e-104">Niektoré bežné problémy, s ktorými sa zákazníci stretávajú, keď Synchronizácia hash hesla nefunguje:</span><span class="sxs-lookup"><span data-stu-id="faf1e-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="faf1e-105">Konto služby Active Directory používané službou Azure AD Connect na komunikáciu s lokálnou službou Active Directory neposkytuje **replikovať zmeny adresárov** a **replikovať zmeny v adresári všetky** povolenia, ktoré sú potrebné na synchronizáciu hesla – musíte tento problém vyriešiť tak, že udelíte tieto povolenia do konta služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="faf1e-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="faf1e-106">Synchronizácia hash hesla je vypnutá, keď správca zmenil používateľa Sign-In metódu z **synchronizácie hesiel** na inú možnosť, ako napríklad **federácia s AD FS** v sprievodcovi Azure AD Connect – tento problém môžete opraviť opätovným zapnutím funkcie **synchronizácie hash hesla** v sprievodcovi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="faf1e-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="faf1e-107">Problém s pripojením s lokálnou službou Active Directory.</span><span class="sxs-lookup"><span data-stu-id="faf1e-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="faf1e-108">Niektoré radiče domén napríklad nie sú prístupné prostredníctvom služby Azure AD Connect, prípadne porty, ktoré [vyžaduje](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) brána firewall, je potrebné vyriešiť tak, že zabezpečíte, že pripojenie medzi SERVEROM Azure AD Connect a lokálnou službou Active Directory funguje správne.</span><span class="sxs-lookup"><span data-stu-id="faf1e-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="faf1e-109">Azure AD Connect server sa momentálne nachádza v režime staging, čo bude mať za následok, že server neumožňuje hash hesla – na vyriešenie problému postupujte podľa krokov uvedených v časti [Riešenie problémov so synchronizáciou hesiel pomocou služby Azure AD Connect Sync – žiadne heslá sa nesynchronizujú](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="faf1e-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="faf1e-110">**Synchronizácia hash hesla nefunguje pre niektorých používateľov**</span><span class="sxs-lookup"><span data-stu-id="faf1e-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="faf1e-111">Ak ste si všimli, že hash hesla sa pre používateľa nesynchronizuje, použite **Riešenie problémov** s úlohou v službe Azure AD Connect, aby sa problém vyriešil.</span><span class="sxs-lookup"><span data-stu-id="faf1e-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="faf1e-112">Vykonajte tieto úlohy:</span><span class="sxs-lookup"><span data-stu-id="faf1e-112">Perform the following tasks:</span></span>

    <span data-ttu-id="faf1e-113">a.</span><span class="sxs-lookup"><span data-stu-id="faf1e-113">a.</span></span> [<span data-ttu-id="faf1e-114">Spustenie úlohy riešenia problémov v sprievodcovi</span><span class="sxs-lookup"><span data-stu-id="faf1e-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="faf1e-115">b.</span><span class="sxs-lookup"><span data-stu-id="faf1e-115">b.</span></span> [<span data-ttu-id="faf1e-116">Použite rutinu typu cmdlet na riešenie problémov a Preskúmajte problém s synchronizáciou hash hesla pre konkrétne použitie.</span><span class="sxs-lookup"><span data-stu-id="faf1e-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="faf1e-117">Lokálny objekt používateľa služby Active Directory je zapnutý, aby **používateľ musel zmeniť heslo pri ďalšom prihlásení** .</span><span class="sxs-lookup"><span data-stu-id="faf1e-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="faf1e-118">Keď je táto možnosť povolená, používateľovi sa priradí dočasné heslo a pri ďalšom prihlásení sa zobrazí výzva na zmenu hesla.</span><span class="sxs-lookup"><span data-stu-id="faf1e-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="faf1e-119">Azure AD Connect nesynchronizuje dočasné heslá na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="faf1e-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="faf1e-120">Ak chcete vyriešiť tento problém, vykonajte jednu z nasledujúcich úloh:</span><span class="sxs-lookup"><span data-stu-id="faf1e-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="faf1e-121">Požiadajte používateľa, aby sa prihlásil do lokálnej aplikácie (napríklad na pracovnej ploche Windowsu), a zmeňte heslo.</span><span class="sxs-lookup"><span data-stu-id="faf1e-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="faf1e-122">Nové heslo sa synchronizuje so službou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="faf1e-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="faf1e-123">Požiadajte správcu o aktualizáciu hesla používateľa bez toho, aby ste museli povoliť používateľovi možnosť pri **ďalšom prihlásení zmeniť heslo** a nové heslo zdieľať s používateľom.</span><span class="sxs-lookup"><span data-stu-id="faf1e-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="faf1e-124">Objekt používateľa lokálnej služby Active Directory **nie je správne nakonfigurovaný** na synchronizáciu objektov alebo synchronizáciu hesla.</span><span class="sxs-lookup"><span data-stu-id="faf1e-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="faf1e-125">Ak chcete vyriešiť tento problém, postupujte podľa krokov uvedených v [téme Riešenie problémov so synchronizáciou hash hesla pomocou služby Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="faf1e-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







