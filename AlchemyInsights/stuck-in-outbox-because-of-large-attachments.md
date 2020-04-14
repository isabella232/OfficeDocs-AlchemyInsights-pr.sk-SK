---
title: Uviazol v priečinku Pošta na odoslanie z dôvodu veľkých príloh
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241267"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="18ee5-102">Oprava správ, ktoré sú prilepené v priečinku Pošta na odoslanie</span><span class="sxs-lookup"><span data-stu-id="18ee5-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="18ee5-103">Odporúčame vám začať spustením scenára ["Mám problémy s odosielaním, prijímaním alebo vyhľadávaním e-mailových správ"](https://aka.ms/SaRA-OutlookSendReceive) z nástroja [technickej podpory a obnovenia programu Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="18ee5-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="18ee5-104">Keď správa uviazne v priečinku Pošta na odoslanie, najpravdepodobnejšou príčinou je veľká príloha alebo možnosť "Odoslať ihneď po pripojení" nie je povolená.</span><span class="sxs-lookup"><span data-stu-id="18ee5-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="18ee5-105">**Odstráňte veľkú prílohu**</span><span class="sxs-lookup"><span data-stu-id="18ee5-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="18ee5-106">V programe Outlook vyberte položku **Odoslať a prijať** > **prácu v režime offline**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="18ee5-107">Na navigačnej table vyberte položku **Pošta na odoslanie**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="18ee5-108">Odtiaľ môžete:</span><span class="sxs-lookup"><span data-stu-id="18ee5-108">From here, you can:</span></span> 
    - <span data-ttu-id="18ee5-109">Odstráňte správu (vyberte ju a potom vyberte položku **Delete**).</span><span class="sxs-lookup"><span data-stu-id="18ee5-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="18ee5-110">Presuňte správu do priečinka Koncepty, dvojitým kliknutím ho otvorte a odstráňte ju vyberte a potom vyberte položku **Delete (odstrániť**).</span><span class="sxs-lookup"><span data-stu-id="18ee5-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="18ee5-111">Ak sa zobrazí chyba, ktorá hovorí, že program Outlook sa pokúša odovzdať správu, zavrite program Outlook.</span><span class="sxs-lookup"><span data-stu-id="18ee5-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="18ee5-112">Ukončenie môže trvať niekoľko okamihov.</span><span class="sxs-lookup"><span data-stu-id="18ee5-112">It may take a few moments to exit.</span></span> <span data-ttu-id="18ee5-113">Ak sa program Outlook nezavrie, stlačte kombináciu klávesov CTRL + ALT + DELETE a vyberte položku **Spustiť správcu úloh**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="18ee5-114">V Správcovi úloh vyberte kartu **procesy** , posuňte sa nadol do programu Outlook. exe a vyberte položku **ukončiť proces**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="18ee5-115">Po zatvorení programu Outlook, reštartujte ho a zopakujte kroky 2 a 3.</span><span class="sxs-lookup"><span data-stu-id="18ee5-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="18ee5-116">Po odstránení prílohy kliknite na položku **Odoslať a prijať** > **prácu v režime offline** a pokračujte v práci online.</span><span class="sxs-lookup"><span data-stu-id="18ee5-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="18ee5-117">Správy tiež uviaznu v priečinku Pošta na odoslanie po kliknutí na tlačidlo **Odoslať**, ale nie ste pripojení.</span><span class="sxs-lookup"><span data-stu-id="18ee5-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="18ee5-118">Kliknite na tlačidlo **Odoslať a prijať** a pozrite sa na tlačidlo **pracovať v režime offline** .</span><span class="sxs-lookup"><span data-stu-id="18ee5-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="18ee5-119">Ak je modrá, ste odpojený.</span><span class="sxs-lookup"><span data-stu-id="18ee5-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="18ee5-120">Kliknutím naň sa pripojíte (tlačidlo sa zmení na bielu) a kliknite na tlačidlo **Odoslať všetko**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="18ee5-121">**Povoliť odosielanie ihneď po pripojení**</span><span class="sxs-lookup"><span data-stu-id="18ee5-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="18ee5-122">Na súbor karte, kliknite na tlačidlo **Možnosti**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="18ee5-123">V dialógovom okne Možnosti programu Outlook kliknite na tlačidlo **Spresniť**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="18ee5-124">V časti Odoslať a prijať kliknutím povoľte **Odoslať ihneď po pripojení**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="18ee5-125">Kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="18ee5-125">Click **OK**.</span></span>
 
<span data-ttu-id="18ee5-126">Podrobné informácie nájdete na:</span><span class="sxs-lookup"><span data-stu-id="18ee5-126">For full details, see:</span></span>
- [<span data-ttu-id="18ee5-127">Video: odoslanie alebo odstránenie uviaznutia e-mailu</span><span class="sxs-lookup"><span data-stu-id="18ee5-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="18ee5-128">E-mail zostane v priečinku Pošta na odoslanie, až kým manuálne nespustíte operáciu odosielania a prijímania v programe Outlook</span><span class="sxs-lookup"><span data-stu-id="18ee5-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
