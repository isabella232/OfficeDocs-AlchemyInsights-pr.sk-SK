---
title: Povolenie archívnej poštovej schránky
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811721"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="f56d7-102">Povolenie archívnej poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="f56d7-102">Enable an archive mailbox</span></span>

<span data-ttu-id="f56d7-103">Ak chcete, aby sme spustili automatizované kontroly na zabezpečenie konfigurácie archívnej poštovej schránky, vyberte tlačidlo späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu konta.</span><span class="sxs-lookup"><span data-stu-id="f56d7-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="f56d7-104">Archívna poštová schránka v Microsoft 365 (nazývané aj *online archívy* alebo *miestne archívy*) poskytuje používateľom ďalšie ukladanie e-mailov.</span><span class="sxs-lookup"><span data-stu-id="f56d7-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="f56d7-105">Používatelia môžu presúvať alebo kopírovať položky do svojej archívnej poštovej schránky a správcovia môžu vytvoriť politiku archivácie, ktorá automaticky premiestni položky do archívnych poštových schránok.</span><span class="sxs-lookup"><span data-stu-id="f56d7-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="f56d7-106">Tu je postup na vytvorenie archívnej poštovej schránky:</span><span class="sxs-lookup"><span data-stu-id="f56d7-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="f56d7-107">Prejdite na [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="f56d7-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="f56d7-108">Prihláste sa do služieb Microsoft 365 pomocou konta správcu.</span><span class="sxs-lookup"><span data-stu-id="f56d7-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="f56d7-109">Na ľavej table &amp; Centra zabezpečenia dodržiavania súladu vyberte položku **Archív správy informácií** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="f56d7-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="f56d7-110">Vyberte používateľa, ktorého archívna poštová schránka chcete povoliť.</span><span class="sxs-lookup"><span data-stu-id="f56d7-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="f56d7-111">Na table s podrobnosťami na pravej strane kliknite na položku **Povoliť** a potom v upozorňujúcej správe kliknite na položku **Áno** , čím sa povolí archívna poštová schránka.</span><span class="sxs-lookup"><span data-stu-id="f56d7-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="f56d7-112">Môžete tiež hromadne povoliť archívnych poštových schránok výberom viacerých používateľov (použitím klávesov **SHIFT** alebo **Ctrl** ) a následným kliknutím na položku **Povoliť** na table s podrobnosťami.</span><span class="sxs-lookup"><span data-stu-id="f56d7-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="f56d7-113">Zdieľané poštové schránky</span><span class="sxs-lookup"><span data-stu-id="f56d7-113">Shared mailboxes</span></span>

<span data-ttu-id="f56d7-114">Ak chcete povoliť Archív pre zdieľanú poštovú schránku, vyžaduje sa licencia na Exchange Online Plan 2 alebo licenciu na Exchange Online Plan 1 s licenciou na archiváciu na Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f56d7-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="f56d7-115">Ak chcete povoliť Archív pre zdieľanú poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="f56d7-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="f56d7-116">Prejdite do [centra spravovania pre Exchange](https://outlook.office365.com/ecp) a prihláste sa pomocou svojho konta správcu.</span><span class="sxs-lookup"><span data-stu-id="f56d7-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="f56d7-117">Prejdite na **Recipients**  >  **zdieľaných**príjemcov.</span><span class="sxs-lookup"><span data-stu-id="f56d7-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="f56d7-118">Vyberte zdieľanú poštovú schránku.</span><span class="sxs-lookup"><span data-stu-id="f56d7-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="f56d7-119">Na table s podrobnosťami na pravej strane **v časti Archív na mieste**kliknite na položku **Povoliť**a potom kliknite na položku **Áno** , čím povolíte archívnu poštovú schránku.</span><span class="sxs-lookup"><span data-stu-id="f56d7-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="f56d7-120">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="f56d7-120">For more information, see:</span></span>
  
- [<span data-ttu-id="f56d7-121">Povolenie archívnych poštových schránok</span><span class="sxs-lookup"><span data-stu-id="f56d7-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="f56d7-122">Nastavenie politiky archivácie a odstraňovania</span><span class="sxs-lookup"><span data-stu-id="f56d7-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
