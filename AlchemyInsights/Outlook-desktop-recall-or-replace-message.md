---
title: Stiahnutie alebo nahradenie e-mailovej správy v aplikácii Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502334"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="1d3ca-102">Vyvolanie alebo nahradenie e-mailovej správy programu Outlook</span><span class="sxs-lookup"><span data-stu-id="1d3ca-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="1d3ca-103">Ako správca si môžete **vyvolať správy v mene používateľov pomocou prostredia PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="1d3ca-104">Správy nemôžete vyvolať z Centra spravovania.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="1d3ca-105">Môžete **si spomenúť len na správy odoslané osobám vo vašej organizácii.**</span><span class="sxs-lookup"><span data-stu-id="1d3ca-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="1d3ca-106">Ak bola napríklad správa odoslaná na adresu Gmail, nemôžete si ju spomenúť.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="1d3ca-107">Správy **odoslané z Outlooku 2016**v počítači môžete vyvolať iba .</span><span class="sxs-lookup"><span data-stu-id="1d3ca-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="1d3ca-108">Ak používateľ odošle správu pomocou Outlooku for Mac alebo Outlooku na webe, nemôžete si ju spomenúť.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="1d3ca-109">Stiahnutie alebo nahradenie e-mailovej správy:</span><span class="sxs-lookup"><span data-stu-id="1d3ca-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="1d3ca-110">Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Odoslaná pošta.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="1d3ca-111">Dvojitým kliknutím otvorte správu, ktorú si chcete vyvolať.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="1d3ca-112">Vyberte kartu **Správa** a potom vyberte položku **Akcie**  >  **Vyvolať túto správu**.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="1d3ca-113">Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo Odstrániť **neprečítané kópie a nahradiť novou správou**a potom vyberte **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="1d3ca-114">Ak odosielate náhradnú správu, napíšte správu a potom vyberte položku **Odoslať**.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="1d3ca-115">Úspech alebo neúspech odvolania správy závisí od nastavení príjemcu v programe Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="1d3ca-116">Postup na kontrolu stiahnutia nájdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="1d3ca-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="1d3ca-117">Vyhľadávanie a odstraňovanie e-mailových správ v organizácii</span><span class="sxs-lookup"><span data-stu-id="1d3ca-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="1d3ca-118">Ak nie ste globálnym správcom, váš účet musí byť pridaný do roly správcu elektronického vyhľadávania alebo roly správy vyhľadávania súladu, aby ste mohli vyhľadávať správy.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="1d3ca-119">Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo rolu správy Vyhľadávania a vymazania.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="1d3ca-120">Povolenia pre tieto roly sú priradené v [centre zabezpečenia a súladu](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="1d3ca-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="1d3ca-121">[Vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhľadajte správu, ktorá sa má odstrániť.</span><span class="sxs-lookup"><span data-stu-id="1d3ca-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="1d3ca-122">[Pripojte sa k PowerShell centra zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="1d3ca-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="1d3ca-123">Ak používate viacnásobné overovanie, pozrite si tému [Pripojenie k prostrediu PowerShell centra zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)pomocou viacnásobného overovania .</span><span class="sxs-lookup"><span data-stu-id="1d3ca-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>