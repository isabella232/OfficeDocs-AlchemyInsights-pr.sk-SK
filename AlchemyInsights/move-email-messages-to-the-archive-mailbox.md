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
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511055"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="c548a-102">Premiestnenie e-mailu do archívnej poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="c548a-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="c548a-103">Skontrolujte, či bola povolená **archívna poštová schránka.**</span><span class="sxs-lookup"><span data-stu-id="c548a-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="c548a-104">Ak nie, použite kroky v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) umožniť archívnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="c548a-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="c548a-105">Ak chcete automaticky archivovať správy do archívnej poštovej schránky, značka uchovávania údajov s akciou **Presunúť do archívu** musí byť nastavená tak, aby sa **automaticky použila na celú značku poštovej schránky (predvolenej).**</span><span class="sxs-lookup"><span data-stu-id="c548a-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="c548a-106">Tu uvedené kroky vytvorte značku: [Predvolená značka archívu](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="c548a-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="c548a-107">Potom pridajte značku **Archív** do politiky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="c548a-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="c548a-108">V Centre spravovania pre Exchange vyberte položku **Politiky uchovávania údajov** > pridať **značku Presunúť do archívu** do politiky > **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="c548a-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="c548a-109">Teraz [priraďte politiku uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) k poštovej schránke konkrétneho používateľa.</span><span class="sxs-lookup"><span data-stu-id="c548a-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="c548a-110">Rovnaká politika sa použije pre **poštovú** schránku Primárne aj **Archív.**</span><span class="sxs-lookup"><span data-stu-id="c548a-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="c548a-111">Môže byť potrebné vynútiť asistenta spravovaných priečinkov (MFA) spustiť a použiť nové nastavenia poštovej schránky používateľa.</span><span class="sxs-lookup"><span data-stu-id="c548a-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="c548a-112">Spustite nasledujúci príkaz, keď [je pripojený k EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustiť Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="c548a-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="c548a-113">Počiatočná Identifikácia programu ManagedFolderAssistant<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="c548a-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="c548a-114">Ďalšie informácie o nastavení politiky archivácie sa nachádzajú v téme [Nastavenie politiky archivácie a odstránenia pre poštové schránky](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="c548a-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  