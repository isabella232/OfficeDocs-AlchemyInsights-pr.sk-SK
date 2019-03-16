---
title: Desktop odvolanie správy programu Outlook alebo nahradiť e-mailovej správy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657058"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="4bf12-102">Odvolanie alebo nahradenie e-mailovej správy</span><span class="sxs-lookup"><span data-stu-id="4bf12-102">Recall or replace an email message</span></span>

- <span data-ttu-id="4bf12-103">Ako admin, môžete **pripomenúť správy v mene používateľov pomocou prostredia PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="4bf12-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="4bf12-104">Nemôže odvolať správy z admin center.</span><span class="sxs-lookup"><span data-stu-id="4bf12-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="4bf12-105">Môžete **len recall správy, ktoré odosielajú ľudí vo vašej organizácii**.</span><span class="sxs-lookup"><span data-stu-id="4bf12-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="4bf12-106">Ak bola odoslaná na adresu služby Gmail, napríklad, nemôžem spomenúť to.</span><span class="sxs-lookup"><span data-stu-id="4bf12-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="4bf12-107">Môžete **len recall správy odoslané z programu Outlook 2016 v počítači**.</span><span class="sxs-lookup"><span data-stu-id="4bf12-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="4bf12-108">Ak používateľ odošle správu pomocou programu Outlook for Mac alebo Outlook na webe, si nemôžete spomenúť.</span><span class="sxs-lookup"><span data-stu-id="4bf12-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="4bf12-109">Ak chcete odvolať alebo nahradiť e-mailovej správy:</span><span class="sxs-lookup"><span data-stu-id="4bf12-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="4bf12-110">Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Sent Items.</span><span class="sxs-lookup"><span data-stu-id="4bf12-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="4bf12-111">Správu chcete odvolať ho otvorte dvojitým kliknutím.</span><span class="sxs-lookup"><span data-stu-id="4bf12-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="4bf12-112">Vyberte **správy** kartu, a potom vyberte **akcie** > **Odvolanie tejto správy**.</span><span class="sxs-lookup"><span data-stu-id="4bf12-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="4bf12-113">Vyberte **Odstrániť neprečítané kópie tejto správy** alebo **Odstrániť neprečítané kópie a nahradiť novú správu**, a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="4bf12-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="4bf12-114">Ak posielate správu náhradné, napísať správu a vyberte položku **Odoslať**.</span><span class="sxs-lookup"><span data-stu-id="4bf12-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="4bf12-115">Úspech či neúspech odvolanie správy závisí od príjemcu nastavenia v programe Outlook.</span><span class="sxs-lookup"><span data-stu-id="4bf12-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="4bf12-116">Kroky na kontrolu, na stiahnutie, nájdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="4bf12-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="4bf12-117">Vyhľadanie a odstránenie e-mailových správ v organizácii</span><span class="sxs-lookup"><span data-stu-id="4bf12-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="4bf12-118">Ak si nie ste globálne admin, váš účet musí pripočítať k eDiscovery Manager úlohu alebo súlad vyhľadávanie rola na vyhľadávanie správ.</span><span class="sxs-lookup"><span data-stu-id="4bf12-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="4bf12-119">Ak chcete odstrániť správy, musíte pripojiť sa k skupine rolí Správa organizácie alebo Hľadať a očistenie rola.</span><span class="sxs-lookup"><span data-stu-id="4bf12-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="4bf12-120">[Centrum zabezpečenia a súladu](https://go.microsoft.com/fwlink/?linkid=2083731)sú priradené povolenia pre tieto úlohy.</span><span class="sxs-lookup"><span data-stu-id="4bf12-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="4bf12-121">[Vytvoriť obsah vyhľadávať](https://docs.microsoft.com/office365/securitycompliance/content-search) správy odstrániť.</span><span class="sxs-lookup"><span data-stu-id="4bf12-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="4bf12-122">[Pripojiť k bezpečnosti a centrum súladu PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="4bf12-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="4bf12-123">Ak používate viacerými autentizácia, nájdete [pripojenie k Office 365 zabezpečenia a súladu centrum PowerShell pomocou viacnásobné overovanie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="4bf12-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>