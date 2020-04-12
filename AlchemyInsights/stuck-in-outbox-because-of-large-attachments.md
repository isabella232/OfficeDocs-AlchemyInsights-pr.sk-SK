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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232645"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="a5482-102">Oprava správ, ktoré sú prilepené v priečinku Pošta na odoslanie</span><span class="sxs-lookup"><span data-stu-id="a5482-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="a5482-103">Odporúčame vám začať spustením scenára ["Mám problémy s odosielaním, prijímaním alebo vyhľadávaním e-mailových správ"](https://aka.ms/SaRA-OutlookSendReceive) z nástroja [technickej podpory a obnovenia programu Microsoft](https://diagnostics.office.com/#/) na postihnutý počítač.</span><span class="sxs-lookup"><span data-stu-id="a5482-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="a5482-104">Keď správa uviazne v priečinku Pošta na odoslanie, najpravdepodobnejšou príčinou je veľká príloha alebo možnosť "Odoslať ihneď po pripojení" nie je povolená.</span><span class="sxs-lookup"><span data-stu-id="a5482-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="a5482-105">**Odstráňte veľkú prílohu**</span><span class="sxs-lookup"><span data-stu-id="a5482-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="a5482-106">Kliknite na položku **Odoslať a prijať** > **prácu v režime offline**.</span><span class="sxs-lookup"><span data-stu-id="a5482-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="a5482-107">Na navigačnej table kliknite na položku **Pošta na odoslanie**.</span><span class="sxs-lookup"><span data-stu-id="a5482-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="a5482-108">Odtiaľ môžete:</span><span class="sxs-lookup"><span data-stu-id="a5482-108">From here, you can:</span></span> 
    - <span data-ttu-id="a5482-109">Odstrániť správu.</span><span class="sxs-lookup"><span data-stu-id="a5482-109">Delete the message.</span></span> <span data-ttu-id="a5482-110">Stačí ho vybrať a kliknite na tlačidlo **odstrániť**.</span><span class="sxs-lookup"><span data-stu-id="a5482-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="a5482-111">Presuňte správu do **priečinka Koncepty**, dvojitým kliknutím otvorte správu a odstráňte prílohu (kliknite naň a kliknite na tlačidlo **odstrániť**).</span><span class="sxs-lookup"><span data-stu-id="a5482-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="a5482-112">Ak sa vám zobrazí chyba, ktorú program Outlook pokúša odovzdať, zavrite program Outlook.</span><span class="sxs-lookup"><span data-stu-id="a5482-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="a5482-113">Ukončenie môže trvať niekoľko okamihov.</span><span class="sxs-lookup"><span data-stu-id="a5482-113">It may take a few moments to exit.</span></span> <span data-ttu-id="a5482-114">Ak sa program Outlook nezavrie, stlačte **kombináciu klávesov CTRL + ALT + DELETE** a kliknite na položku **Spustiť správcu úloh**.</span><span class="sxs-lookup"><span data-stu-id="a5482-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="a5482-115">V Správcovi úloh vyberte kartu **procesy** , posuňte sa nadol na položku Outlook. exe a kliknite na tlačidlo **ukončiť proces**.</span><span class="sxs-lookup"><span data-stu-id="a5482-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="a5482-116">Po zatvorení programu Outlook reštartujte program Outlook a zopakujte kroky 2-3.</span><span class="sxs-lookup"><span data-stu-id="a5482-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="a5482-117">Po odstránení prílohy kliknite na položku **Odoslať a prijať** > **prácu v režime offline** a zrušte výber tlačidla a pokračujte v práci online.</span><span class="sxs-lookup"><span data-stu-id="a5482-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="a5482-118">Správy tiež uviaznu v priečinku Pošta na odoslanie po kliknutí na tlačidlo **Odoslať**, ale nie ste pripojení.</span><span class="sxs-lookup"><span data-stu-id="a5482-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="a5482-119">Kliknite na tlačidlo **Odoslať a prijať** a pozrite sa na tlačidlo **pracovať v režime offline** .</span><span class="sxs-lookup"><span data-stu-id="a5482-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="a5482-120">Ak je modrá, ste odpojený.</span><span class="sxs-lookup"><span data-stu-id="a5482-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="a5482-121">Kliknutím naň sa pripojíte (tlačidlo sa zmení na bielu) a kliknite na tlačidlo **Odoslať všetko**.</span><span class="sxs-lookup"><span data-stu-id="a5482-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="a5482-122">**Povoliť odosielanie ihneď po pripojení**</span><span class="sxs-lookup"><span data-stu-id="a5482-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="a5482-123">Na súbor karte, kliknite na tlačidlo **Možnosti**.</span><span class="sxs-lookup"><span data-stu-id="a5482-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="a5482-124">V dialógovom okne Možnosti programu Outlook kliknite na tlačidlo **Spresniť**.</span><span class="sxs-lookup"><span data-stu-id="a5482-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="a5482-125">V časti Odoslať a prijať kliknutím povoľte **Odoslať ihneď po pripojení**.</span><span class="sxs-lookup"><span data-stu-id="a5482-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="a5482-126">Kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="a5482-126">Click **OK**.</span></span>
 
<span data-ttu-id="a5482-127">Podrobné informácie nájdete na:</span><span class="sxs-lookup"><span data-stu-id="a5482-127">For full details, see:</span></span>
- [<span data-ttu-id="a5482-128">Video: odoslanie alebo odstránenie uviaznutia e-mailu</span><span class="sxs-lookup"><span data-stu-id="a5482-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="a5482-129">E-mail zostane v priečinku Pošta na odoslanie, až kým manuálne nespustíte operáciu odosielania a prijímania v programe Outlook</span><span class="sxs-lookup"><span data-stu-id="a5482-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
