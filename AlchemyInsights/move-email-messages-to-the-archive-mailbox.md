---
title: Presun e-mailových správ do archívnej poštovej schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822177"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="31b55-102">Presunutie e-mailu do archívnej poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="31b55-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="31b55-103">Skontrolujte, či bola povolená **archívna poštová schránka** .</span><span class="sxs-lookup"><span data-stu-id="31b55-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="31b55-104">Ak nie, použite kroky v [tomto článku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) na povolenie archívnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="31b55-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="31b55-105">Ak chcete archivovať správy automaticky do archívnej poštovej schránky, značka uchovávania údajov s akciou **premiestniť do archívu** musí byť nastavená tak, aby sa **automaticky uplatňovala na celú poštovú schránku (predvolenú) značku**.</span><span class="sxs-lookup"><span data-stu-id="31b55-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="31b55-106">Pomocou krokov tu vytvorte Tag: [Archivovať predvolenú značku](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="31b55-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="31b55-107">Potom pridajte **archívnu** značku do politiky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="31b55-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="31b55-108">Exchange Admin Center, vyberte **politiky uchovávania údajov** > pridať **presunúť do archívu Tag** politiky > **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="31b55-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="31b55-109">Teraz [priraďte politiku uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrétnej poštovej schránke používateľa.</span><span class="sxs-lookup"><span data-stu-id="31b55-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="31b55-110">Rovnaká politika sa použije ako **primárna** aj **archívna** poštová schránka.</span><span class="sxs-lookup"><span data-stu-id="31b55-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="31b55-111">Môže byť potrebné vynútiť Asistenta spravovaných priečinkov (MFA) spustiť a použiť nové nastavenia poštovej schránky používateľa.</span><span class="sxs-lookup"><span data-stu-id="31b55-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="31b55-112">Spustite nasledujúci príkaz pri [pripojení k EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustiť Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="31b55-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="31b55-113">Štart-ManagedFolderAssistant-identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="31b55-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="31b55-114">Ďalšie informácie o nastavení politiky archivácie nájdete [v téme Nastavenie politiky archivácie a odstránenia poštových schránok](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="31b55-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  