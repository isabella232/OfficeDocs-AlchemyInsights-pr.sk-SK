---
title: Pridanie alebo odstránenie delegáta v Outlooku pre Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573571"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="a2a60-102">Pridanie alebo odstránenie delegáta v Outlooku pre Windows</span><span class="sxs-lookup"><span data-stu-id="a2a60-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="a2a60-103">Pridanie delegáta v Outlooku pre Windows:</span><span class="sxs-lookup"><span data-stu-id="a2a60-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="a2a60-104">Kliknite na kartu **súbor** a potom na položku **Nastavenie konta** a potom vyberte položku **prístup delegátov**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="a2a60-105">Kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-105">Click on **Add**.</span></span> <span data-ttu-id="a2a60-106">Ak sa **Pridanie** nezobrazuje, v Outlooku a Exchangei nemusí existovať aktívne pripojenie.</span><span class="sxs-lookup"><span data-stu-id="a2a60-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="a2a60-107">V stavovom riadku Outlooku sa zobrazuje stav pripojenia.</span><span class="sxs-lookup"><span data-stu-id="a2a60-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="a2a60-108">Zadajte meno osoby, ktorú chcete označiť ako delegáta, alebo vyhľadajte a vyberte názov v zozname výsledkov hľadania.</span><span class="sxs-lookup"><span data-stu-id="a2a60-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a2a60-109">Delegát musí byť osobou v globálnom zozname adries v organizácii Exchange (GAL).</span><span class="sxs-lookup"><span data-stu-id="a2a60-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="a2a60-110">Kliknite na položku **Pridať** a potom na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="a2a60-111">V dialógovom okne **povolenia delegáta** prijmite predvolené nastavenia povolení alebo vyberte vlastné úrovne prístupu pre priečinky Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2a60-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="a2a60-112">Ak delegát potrebuje povolenie na prácu iba pri žiadostiach o schôdzu a odpovediach, predvolené nastavenia povolení, ako napríklad **delegát, prijímajú kópie správ súvisiacich so schôdzami, ktoré mi boli zaslané** .</span><span class="sxs-lookup"><span data-stu-id="a2a60-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="a2a60-113">Nastavenie povolení pre **doručenú poštu** môžete ponechať na **žiadnej**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="a2a60-114">Žiadosti o schôdzu a odpovede sa presunú priamo do priečinka Doručená pošta delegáta.</span><span class="sxs-lookup"><span data-stu-id="a2a60-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a2a60-115">Na základe predvoleného nastavenia je delegátovi poskytnutý **Editor (môže čítať, vytvárať a upravovať položky)** povolenie pre priečinok **kalendára** .</span><span class="sxs-lookup"><span data-stu-id="a2a60-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="a2a60-116">Keď delegát odpovie na schôdzu vo vašom mene, automaticky sa pridá do priečinka **Kalendár** .</span><span class="sxs-lookup"><span data-stu-id="a2a60-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="a2a60-117">Ak chcete odoslať správu s cieľom informovať delegáta o zmenených povoleniach, začiarknite políčko **automaticky odoslať správu delegátovi so súhrnom týchto povolení** .</span><span class="sxs-lookup"><span data-stu-id="a2a60-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="a2a60-118">Ak chcete, začiarknite políčko **delegát môže zobraziť moje súkromné položky** .</span><span class="sxs-lookup"><span data-stu-id="a2a60-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="a2a60-119">Toto nastavenie ovplyvní všetky priečinky Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2a60-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="a2a60-120">Toto zahŕňa všetky priečinky pošta, kontakty, kalendár, úlohy, poznámky a denník.</span><span class="sxs-lookup"><span data-stu-id="a2a60-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="a2a60-121">Neexistuje spôsob, ako udeliť prístup k súkromným položkám iba do zadaných priečinkov.</span><span class="sxs-lookup"><span data-stu-id="a2a60-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="a2a60-122">Vyberte **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="a2a60-123">Správy odoslané s povoleniami Odoslať v mene zahŕňajú delegáta aj mená vedľa položky **od**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="a2a60-124">Keď sa správa odošle s povoleniami Odoslať ako, zobrazí sa len vaše meno.</span><span class="sxs-lookup"><span data-stu-id="a2a60-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="a2a60-125">Keď pridáte niekoho ako delegáta, môžete pridať poštovú schránku Exchange do svojho profilu v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="a2a60-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="a2a60-126">Pokyny nájdete v téme [spravovanie pošty a položiek kalendára inej osoby](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="a2a60-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="a2a60-127">Ak chcete odstrániť delegáta v Outlooku pre Windows:</span><span class="sxs-lookup"><span data-stu-id="a2a60-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="a2a60-128">Kliknite na kartu **súbor** .</span><span class="sxs-lookup"><span data-stu-id="a2a60-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="a2a60-129">Kliknite na položku **Nastavenie konta** a potom na položku **prístup delegáta**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="a2a60-130">Vyberte meno delegáta, pre ktorého chcete zmeniť povolenia, a potom kliknite na tlačidlo **odstrániť** , za ktorým nasleduje **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="a2a60-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
