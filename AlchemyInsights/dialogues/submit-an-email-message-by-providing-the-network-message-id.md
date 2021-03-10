---
title: Odoslanie e-mailovej správy poskytnutím identifikácie sieťovej správy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695382"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="99e14-102">Odoslanie e-mailovej správy poskytnutím identifikácie sieťovej správy</span><span class="sxs-lookup"><span data-stu-id="99e14-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="99e14-103">V rozbaľovacom zozname **nové odoslanie** vyberte položku **E-mail** a **Identifikácia sieťovej správy**.</span><span class="sxs-lookup"><span data-stu-id="99e14-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="99e14-104">Ak chcete vyhľadať identifikáciu správy e-mailovej správy v Outlooku, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="99e14-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="99e14-105">Dvakrát kliknite na e-mailovú správu, aby sa otvorila.</span><span class="sxs-lookup"><span data-stu-id="99e14-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="99e14-106">Vyberte položku  >  **Vlastnosti** súboru.</span><span class="sxs-lookup"><span data-stu-id="99e14-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="99e14-107">Otvorte Poznámkový blok alebo prázdny wordový dokument a potom skopírujte a prilepte obsah, ktorý sa nachádza v poli **internetové hlavičky** , do otvoreného dokumentu, aby ste mohli lepšie zviditeľniť.</span><span class="sxs-lookup"><span data-stu-id="99e14-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="99e14-108">Vyhľadajte pole **X-MS-Exchange-Organization-Network – ID správy** .</span><span class="sxs-lookup"><span data-stu-id="99e14-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="99e14-109">Hodnota za hodnotou **:** je identifikácia, ktorú potrebujete na odoslanie.</span><span class="sxs-lookup"><span data-stu-id="99e14-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="99e14-110">Ak v časti **Príjemcovia** e-mail pristál v priečinku Nevyžiadaná pošta pre všetkých príjemcov tohto e-mailu, vyberte **položku vybrať všetko**.</span><span class="sxs-lookup"><span data-stu-id="99e14-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="99e14-111">Ak nie, vyberte možnosť len používateľa, ktorý ohlásil problém.</span><span class="sxs-lookup"><span data-stu-id="99e14-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="99e14-112">Ak ste v časti **dôvod na odoslanie** vybrali **možnosť zablokovať**, zadajte, či má byť správa zablokovaná ako **Nevyžiadaná pošta**, **neoprávnené získavanie údajov** alebo **malware**, a potom vyberte položku **Odoslať**.</span><span class="sxs-lookup"><span data-stu-id="99e14-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="99e14-113">Ďalšie informácie nájdete v téme [odoslanie podozrenia na nevyžiadanú poštu, Phish, URL adresy a súbory do spoločnosti Microsoft na skenovanie](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="99e14-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
