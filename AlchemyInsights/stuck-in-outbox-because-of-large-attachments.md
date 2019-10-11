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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441320"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="d89e7-102">Oprava správ, ktoré sú prilepené v priečinku Pošta na odoslanie</span><span class="sxs-lookup"><span data-stu-id="d89e7-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="d89e7-103">Odporúčame vám začať spustením scenára ["Mám problémy s odosielaním, prijímaním alebo vyhľadávaním e-mailových správ"](https://aka.ms/SaRA-OutlookSendReceive) z nástroja [technickej podpory a obnovenia programu Microsoft](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="d89e7-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="d89e7-104">Keď správa uviazne v priečinku Pošta na odoslanie, Najpravdepodobnejšie príčiny sú:</span><span class="sxs-lookup"><span data-stu-id="d89e7-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="d89e7-105">Veľké prílohy.</span><span class="sxs-lookup"><span data-stu-id="d89e7-105">Large attachments.</span></span>
- <span data-ttu-id="d89e7-106">Možnosť **Odoslať okamžite po pripojení** nie je povolená.</span><span class="sxs-lookup"><span data-stu-id="d89e7-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="d89e7-107">Ak chcete odstrániť veľké prílohy:</span><span class="sxs-lookup"><span data-stu-id="d89e7-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="d89e7-108">V programe Outlook vyberte položku **Odoslať a prijať** > **prácu v režime offline**.</span><span class="sxs-lookup"><span data-stu-id="d89e7-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="d89e7-109">Na navigačnej table vyberte položku **Pošta na odoslanie**.</span><span class="sxs-lookup"><span data-stu-id="d89e7-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="d89e7-110">Odtiaľ môžete:</span><span class="sxs-lookup"><span data-stu-id="d89e7-110">From here, you can:</span></span> 
    - <span data-ttu-id="d89e7-111">Odstráňte správu (vyberte ju a potom vyberte položku **Delete**).</span><span class="sxs-lookup"><span data-stu-id="d89e7-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="d89e7-112">Presuňte správu do priečinka Koncepty, dvojitým kliknutím ho otvorte a odstráňte ju vyberte a potom vyberte položku **Delete (odstrániť**).</span><span class="sxs-lookup"><span data-stu-id="d89e7-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="d89e7-113">Ak sa zobrazí chyba, ktorá hovorí, že program Outlook sa pokúša odovzdať správu, zavrite program Outlook.</span><span class="sxs-lookup"><span data-stu-id="d89e7-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="d89e7-114">Ukončenie môže trvať niekoľko okamihov.</span><span class="sxs-lookup"><span data-stu-id="d89e7-114">It may take a few moments to exit.</span></span> <span data-ttu-id="d89e7-115">Ak sa program Outlook nezavrie, stlačte kombináciu klávesov CTRL + ALT + DELETE a vyberte položku **Spustiť správcu úloh**.</span><span class="sxs-lookup"><span data-stu-id="d89e7-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="d89e7-116">V Správcovi úloh vyberte kartu **procesy** , posuňte sa nadol do programu Outlook. exe a vyberte položku **ukončiť proces**.</span><span class="sxs-lookup"><span data-stu-id="d89e7-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="d89e7-117">Po zatvorení programu Outlook, reštartujte ho a zopakujte kroky 2 a 3.</span><span class="sxs-lookup"><span data-stu-id="d89e7-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="d89e7-118">Po odstránení prílohy kliknite na položku **Odoslať a prijať** > **prácu v režime offline** a pokračujte v práci online.</span><span class="sxs-lookup"><span data-stu-id="d89e7-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="d89e7-119">Správy tiež uviaznu v priečinku Pošta na odoslanie po kliknutí na tlačidlo **Odoslať**, ale nie ste pripojení.</span><span class="sxs-lookup"><span data-stu-id="d89e7-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="d89e7-120">Kliknite na tlačidlo **Odoslať a prijať** a pozrite sa na tlačidlo **pracovať v režime offline** .</span><span class="sxs-lookup"><span data-stu-id="d89e7-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="d89e7-121">Ak je modrá, ste odpojený.</span><span class="sxs-lookup"><span data-stu-id="d89e7-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="d89e7-122">Vyberte ho pre pripojenie (tlačidlo sa zmení na bielu) a kliknite na tlačidlo **Odoslať všetko**.</span><span class="sxs-lookup"><span data-stu-id="d89e7-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="d89e7-123">Ak chcete povoliť **odosielanie ihneď po pripojení**:</span><span class="sxs-lookup"><span data-stu-id="d89e7-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="d89e7-124">Vyberte \*\*\*\* > \*\*\*\* možnosti >  súboru**Rozšírené**.</span><span class="sxs-lookup"><span data-stu-id="d89e7-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="d89e7-125">V časti **Odoslať a prijať** vyberte položku **Odoslať ihneď po pripojení**a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="d89e7-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="d89e7-126">Podrobné informácie nájdete na:</span><span class="sxs-lookup"><span data-stu-id="d89e7-126">For full details see:</span></span>
- [<span data-ttu-id="d89e7-127">Video: odoslanie alebo odstránenie uviaznutia e-mailu</span><span class="sxs-lookup"><span data-stu-id="d89e7-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="d89e7-128">E-mail zostane v priečinku Pošta na odoslanie, až kým manuálne nespustíte operáciu odosielania a prijímania v programe Outlook</span><span class="sxs-lookup"><span data-stu-id="d89e7-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
