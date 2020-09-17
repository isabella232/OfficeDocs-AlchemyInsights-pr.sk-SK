---
title: Premiestnenie e-mailových správ do archívnej poštovej schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799795"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="e2b76-102">Premiestnenie e-mailu do archívnej poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="e2b76-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="e2b76-103">Ak chcete, aby sme spustili automatizované kontroly nižšie uvedených nastavení, vyberte tlačidlo späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s premiestnením e-mailov do svojej archívnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="e2b76-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="e2b76-104">Potvrďte, že je povolená **archívna poštová schránka** .</span><span class="sxs-lookup"><span data-stu-id="e2b76-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="e2b76-105">Ak nie, použite postup v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) na povolenie archívnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="e2b76-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="e2b76-106">Ak chcete automaticky archivovať správy do archívnej poštovej schránky, značka uchovávania údajov s akciou **premiestniť do archívu** musí byť nastavená na možnosť **automaticky použiť na celú poštovú schránku (predvolená)**.</span><span class="sxs-lookup"><span data-stu-id="e2b76-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="e2b76-107">Ak chcete vytvoriť značku, postupujte podľa týchto krokov: [Predvolená značka archivácie](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="e2b76-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="e2b76-108">Potom pridajte značku **archivácie** do politiky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="e2b76-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="e2b76-109">V centre spravovania pre Exchange vyberte položku **politiky uchovávania údajov** > pridať **značku premiestniť do archívu** do politiky > **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="e2b76-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="e2b76-110">Teraz [priraďte politiku uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) k poštovej schránke konkrétneho používateľa.</span><span class="sxs-lookup"><span data-stu-id="e2b76-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="e2b76-111">Rovnaká politika sa použije na **primárnu** aj **archívnu** poštovú schránku.</span><span class="sxs-lookup"><span data-stu-id="e2b76-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="e2b76-112">Môže byť potrebné vynútiť Spustenie Asistenta pre spravované priečinky (MFA) a použiť nové nastavenia v poštovej schránke používateľa.</span><span class="sxs-lookup"><span data-stu-id="e2b76-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="e2b76-113">Spustite nasledujúci príkaz pri [pripojení k EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) na spustenie Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="e2b76-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="e2b76-114">Začiatok – ManagedFolderAssistant – identita <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="e2b76-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="e2b76-115">Ďalšie informácie o nastavení politiky archivácie nájdete v téme [Nastavenie politiky archivácie a odstraňovania poštových schránok](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="e2b76-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  