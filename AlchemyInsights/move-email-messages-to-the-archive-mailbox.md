---
title: Premiestnenie e-mailových správ do archívnej poštovej schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522786"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="7b1ba-102">Premiestnenie e-mailu do archívnej poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="7b1ba-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="7b1ba-103">Ak chcete, aby sme spúšťali automatizované kontroly nastavení uvedených nižšie, vyberte tlačidlo Späť < -- v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s presunom e-mailov do archívnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="7b1ba-104">Potvrďte, že **archívna poštová** schránka bola povolená.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="7b1ba-105">Ak nie, použite kroky v tomto [článku umožniť archívnej](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="7b1ba-106">Ak chcete automaticky archivovať správy do archívnej poštovej schránky, značka uchovávania údajov s **akciou Premiestniť** do archívu musí byť nastavená **tak, aby sa automaticky použila na celú značku poštovej schránky (predvolenej)**.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="7b1ba-107">Ak chcete vytvoriť značku, použite kroky na vytvorenie [značky: Archivovať predvolenú značku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="7b1ba-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="7b1ba-108">Potom pridajte značku **Archivovať** do politiky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="7b1ba-109">V Centre spravovania pre Exchange vyberte **položku Politiky** uchovávania > **pridajte značku Presunúť** do archívu do politiky > **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="7b1ba-110">Teraz [priraďte politiku uchovávania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) údajov k poštovej schránke konkrétneho používateľa.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="7b1ba-111">Rovnaká politika sa použije na poštovú schránku **Primárne** aj **Archív.**</span><span class="sxs-lookup"><span data-stu-id="7b1ba-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="7b1ba-112">Môže byť potrebné vynútiť Asistenta pre spravované priečinky (MFA) spustiť a použiť nové nastavenia poštovej schránky používateľa.</span><span class="sxs-lookup"><span data-stu-id="7b1ba-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="7b1ba-113">Spustite nasledujúci príkaz pri pripojení [k EXO PowerShell spustiť](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="7b1ba-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="7b1ba-114">Štart-ManagedFolderAssistant -Identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="7b1ba-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="7b1ba-115">Ďalšie informácie o nastavení politiky archivácie nájdete v téme [Nastavenie politiky archivácie a odstránenia poštových schránok](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="7b1ba-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  