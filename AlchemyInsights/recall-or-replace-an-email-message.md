---
title: Odvolanie alebo nahradenie e-mailovej správy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799219"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="5c8de-102">Odvolanie alebo nahradenie e-mailovej správy v programe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5c8de-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="5c8de-103">Môžete **vyvolať iba správy, ktoré sa odosielajú ľuďom vo vašej organizácii**.</span><span class="sxs-lookup"><span data-stu-id="5c8de-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="5c8de-104">Ak bola správa odoslaná na adresu služby Gmail, môžete ju napríklad vyvolať.</span><span class="sxs-lookup"><span data-stu-id="5c8de-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="5c8de-105">Môžete **odvolať len správy odoslané z outlooku 2016 pre PC**.</span><span class="sxs-lookup"><span data-stu-id="5c8de-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="5c8de-106">Ak používateľ odošle správu pomocou Outlooku pre Mac alebo Outlooku na webe, nemôžete ju vyvolať.</span><span class="sxs-lookup"><span data-stu-id="5c8de-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="5c8de-107">Ak ste **správcom, môžete v mene používateľov odvolať správy pomocou prostredia PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="5c8de-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="5c8de-108">Správy nemožno odvolať z centra spravovania.</span><span class="sxs-lookup"><span data-stu-id="5c8de-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="5c8de-109">Ďalšie informácie nájdete v časti Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="5c8de-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="5c8de-110">**Odvolanie alebo nahradenie e-mailovej správy, ktorú ste odoslali**</span><span class="sxs-lookup"><span data-stu-id="5c8de-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="5c8de-111">Na table priečinok v ľavej časti okna Outlooku vyberte priečinok Odoslaná pošta.</span><span class="sxs-lookup"><span data-stu-id="5c8de-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="5c8de-112">Otvorte správu, ktorú chcete odvolať.</span><span class="sxs-lookup"><span data-stu-id="5c8de-112">Open the message that you want to recall.</span></span> <span data-ttu-id="5c8de-113">Ak chcete správu otvoriť, musíte dvakrát kliknúť.</span><span class="sxs-lookup"><span data-stu-id="5c8de-113">You must double-click to open the message.</span></span> <span data-ttu-id="5c8de-114">Ak vyberiete správu tak, aby sa zobrazila na table na čítanie, nebudete môcť správu odvolať.</span><span class="sxs-lookup"><span data-stu-id="5c8de-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="5c8de-115">Na karte Správa vyberte položku **akcie**  >  **odvolať túto správu**.</span><span class="sxs-lookup"><span data-stu-id="5c8de-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="5c8de-116">Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo **Odstrániť neprečítané kópie a nahradiť ich novou správou a**potom vyberte **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="5c8de-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="5c8de-117">Ak odosielate náhradnú správu, Vytvorte správu a potom vyberte položku **Odoslať**.</span><span class="sxs-lookup"><span data-stu-id="5c8de-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="5c8de-118">Úspešné alebo neúspešné odvolanie správy závisí od nastavení príjemcov v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="5c8de-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="5c8de-119">Ďalšie informácie vrátane informácií o tom, ako skontrolovať odvolanie, nájdete v téme [odvolanie alebo nahradenie e-mailovej správy, ktorú ste odoslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="5c8de-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="5c8de-120">***Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii*** Ak chcete vyhľadať a odstrániť e-mailové správy vo vašej organizácii, je to najjednoduchšie, ak ste globálnym správcom. Ak nie ste globálnym správcom, vaše konto sa musí pridať do skupiny rolí správcu eDiscovery alebo na rolu riadenia vyhľadávania súladu.</span><span class="sxs-lookup"><span data-stu-id="5c8de-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="5c8de-121">Ak chcete odstrániť správy, budete sa musieť zapojiť do skupiny rolí Správa organizácie alebo do roly riadenia vyhľadávania a čistenia.</span><span class="sxs-lookup"><span data-stu-id="5c8de-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="5c8de-122">Povolenia pre tieto roly sa priraďujú v [Centre zabezpečenia & Compliance](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="5c8de-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="5c8de-123">Ak chcete nájsť správu, ktorú chcete odstrániť, [vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="5c8de-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="5c8de-124">[Pripojte sa k zabezpečeniu & prostredie centrum dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="5c8de-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="5c8de-125">Ak používate MFA, prečítajte si tému [pripojenie k službe Microsoft 365 security & centrum dodržiavania súladu s použitím viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="5c8de-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
