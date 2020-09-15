---
title: Stiahnutie alebo nahradenie e-mailovej správy v Outlooku v počítači
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664005"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="d5728-102">Odvolanie alebo nahradenie e-mailovej správy v Outlooku</span><span class="sxs-lookup"><span data-stu-id="d5728-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="d5728-103">Ako správca môžete **odvolať správy v mene používateľov, ktorí používajú prostredie PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="d5728-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="d5728-104">Správy nemožno odvolať z centra spravovania.</span><span class="sxs-lookup"><span data-stu-id="d5728-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="d5728-105">Môžete **vyvolať iba správy, ktoré sa odosielajú ľuďom vo vašej organizácii**.</span><span class="sxs-lookup"><span data-stu-id="d5728-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="d5728-106">Ak bola správa odoslaná na adresu služby Gmail, môžete ju napríklad vyvolať.</span><span class="sxs-lookup"><span data-stu-id="d5728-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="d5728-107">**Správy odoslané z outlooku 2016 v PC môžete vyvolať len**.</span><span class="sxs-lookup"><span data-stu-id="d5728-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="d5728-108">Ak používateľ odošle správu pomocou Outlooku pre Mac alebo Outlooku na webe, nemôžete ju vyvolať.</span><span class="sxs-lookup"><span data-stu-id="d5728-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="d5728-109">Odvolanie alebo nahradenie e-mailovej správy:</span><span class="sxs-lookup"><span data-stu-id="d5728-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="d5728-110">Na table priečinok v ľavej časti okna Outlooku vyberte priečinok Odoslaná pošta.</span><span class="sxs-lookup"><span data-stu-id="d5728-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="d5728-111">Dvojitým kliknutím otvorte správu, ktorú chcete vyvolať.</span><span class="sxs-lookup"><span data-stu-id="d5728-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="d5728-112">Vyberte kartu **Správa** a potom vyberte položku **akcie**  >  **odvolať túto správu**.</span><span class="sxs-lookup"><span data-stu-id="d5728-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="d5728-113">Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo **Odstrániť neprečítané kópie a nahradiť ich novou správou**a potom vyberte **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="d5728-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="d5728-114">Ak odosielate náhradnú správu, Vytvorte správu a potom vyberte položku **Odoslať**.</span><span class="sxs-lookup"><span data-stu-id="d5728-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="d5728-115">Úspech alebo neúspech odvolania správy závisí od nastavení príjemcu v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="d5728-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="d5728-116">Postup na kontrolu odvolania nájdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="d5728-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="d5728-117">Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii</span><span class="sxs-lookup"><span data-stu-id="d5728-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="d5728-118">Ak nie ste globálnym správcom, konto sa musí pridať do roly správcu eDiscovery alebo na rolu správy vyhľadávania súladu, aby ste mohli vyhľadávať správy.</span><span class="sxs-lookup"><span data-stu-id="d5728-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="d5728-119">Ak chcete odstrániť správy, budete sa musieť zapojiť do skupiny rolí Správa organizácie alebo do roly riadenia vyhľadávania a čistenia.</span><span class="sxs-lookup"><span data-stu-id="d5728-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="d5728-120">Povolenia pre tieto roly sa priraďujú v [Centre zabezpečenia a dodržiavania súladu](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="d5728-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="d5728-121">Ak chcete nájsť správu, ktorú chcete odstrániť, [vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="d5728-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="d5728-122">[Pripojenie k centru PowerShell zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d5728-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="d5728-123">Ak používate viacnásobné overovanie, pozrite si tému [pripojenie k PowerShell v centre zabezpečenia a dodržiavania súladu so službou Microsoft 365 s použitím viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d5728-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>