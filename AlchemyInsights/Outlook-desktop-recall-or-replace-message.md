---
title: Outlook Desktop Recall alebo nahradiť e-mailovú správu
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496126"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="cab49-102">Vyvolanie alebo nahradenie e-mailovej správy programu Outlook</span><span class="sxs-lookup"><span data-stu-id="cab49-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="cab49-103">Ako admin, môžete **pripomenúť správy v mene používateľov pomocou PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="cab49-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="cab49-104">Správy z centra spravovania nemožno vyvolať.</span><span class="sxs-lookup"><span data-stu-id="cab49-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="cab49-105">Môžete **pripomenúť iba správy odoslané ľuďom vo vašej organizácii**.</span><span class="sxs-lookup"><span data-stu-id="cab49-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="cab49-106">Ak bola správa odoslaná na adresu služby Gmail, nemôžete ju napríklad pripomenúť.</span><span class="sxs-lookup"><span data-stu-id="cab49-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="cab49-107">Môžete si **len pripomenúť správy odoslané z programu Outlook 2016 na PC**.</span><span class="sxs-lookup"><span data-stu-id="cab49-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="cab49-108">Ak používateľ odošle správu pomocou programu Outlook for Mac alebo Outlook na webe, nemôžete pripomenúť.</span><span class="sxs-lookup"><span data-stu-id="cab49-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="cab49-109">Ak chcete pripomenúť alebo nahradiť e-mailovú správu:</span><span class="sxs-lookup"><span data-stu-id="cab49-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="cab49-110">Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Odoslaná pošta.</span><span class="sxs-lookup"><span data-stu-id="cab49-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="cab49-111">Dvakrát kliknite na správu, ktorú chcete pripomenúť, aby ste ju otvorili.</span><span class="sxs-lookup"><span data-stu-id="cab49-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="cab49-112">Vyberte kartu **Správa** a potom vyberte **akcie** > **vyvolanie tejto správy**.</span><span class="sxs-lookup"><span data-stu-id="cab49-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="cab49-113">Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo **odstráňte neprečítané kópie a nahraďte ju novou správou**a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="cab49-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="cab49-114">Ak odosielate náhradnú správu, Vytvorte správu a potom vyberte položku **Odoslať**.</span><span class="sxs-lookup"><span data-stu-id="cab49-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="cab49-115">Úspech alebo neúspech odvolanie správy závisí od nastavenia príjemcu v programe Outlook.</span><span class="sxs-lookup"><span data-stu-id="cab49-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="cab49-116">Postup na kontrolu stiahnutia z trhu nájdete [v tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="cab49-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="cab49-117">Vyhľadávanie a odstraňovanie e-mailových správ vo vašej organizácii</span><span class="sxs-lookup"><span data-stu-id="cab49-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="cab49-118">Ak nie ste globálny správca, konto sa musí pridať do roly správcu eDiscovery alebo roly správy vyhľadávania súladu, aby ste mohli vyhľadávať správy.</span><span class="sxs-lookup"><span data-stu-id="cab49-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="cab49-119">Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo k úlohe správy vyhľadávania a čistenia.</span><span class="sxs-lookup"><span data-stu-id="cab49-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="cab49-120">Povolenia pre tieto roly sú priradené v [Centre zabezpečenia a súladu](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="cab49-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="cab49-121">[Vytvorte hľadanie obsahu](https://docs.microsoft.com/office365/securitycompliance/content-search) a vyhľadajte správu, ktorá sa má odstrániť.</span><span class="sxs-lookup"><span data-stu-id="cab49-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="cab49-122">[Pripojiť k zabezpečenia a súladu centrum PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="cab49-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="cab49-123">Ak používate viacnásobné overovanie, pozrite si [pripojenie k Office 365 zabezpečenia a súladu centrum PowerShell pomocou viacnásobné overovanie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="cab49-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>