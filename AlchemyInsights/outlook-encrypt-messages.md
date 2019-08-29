---
title: S/MIME v programe Outlook na webe
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666855"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="83fc6-102">Šifrovanie e-mailových správ v programe Outlook</span><span class="sxs-lookup"><span data-stu-id="83fc6-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="83fc6-103">Šifrovanie správ v Office 365 je postavený na Microsoft Azure Rights Management (Azure RMS), ktorá je súčasťou Azure ochranu informácií.</span><span class="sxs-lookup"><span data-stu-id="83fc6-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="83fc6-104">Ak vaše predplatné obsahuje Azure Rights Management alebo Azure ochrana informácií, **nie je potrebné podniknúť akékoľvek opatrenia manuálne povoliť alebo aktivovať** správy prístupových práv.</span><span class="sxs-lookup"><span data-stu-id="83fc6-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="83fc6-105">Na základe spätnej väzby od zákazníkov, sme sa už umožňujúce Exchange mail tok pravidiel na automatické šifrovanie odchádzajúce e-mail obsahujúci určitý druh citlivé informácie v nájomcu v predvolenom nastavení.</span><span class="sxs-lookup"><span data-stu-id="83fc6-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="83fc6-106">Namiesto toho poskytujeme podrobné pokyny o ako môžete tak urobiť sami.</span><span class="sxs-lookup"><span data-stu-id="83fc6-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="83fc6-107">Ďalšie podrobnosti o tom, ako vytvoriť pravidlo dopravy šifrovať citlivé údaje, nájdete v [tomto článku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="83fc6-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="83fc6-108">Ak používate program Outlook na webe (predtým **OWA**): pri písaní e-mailovej správy, stačí kliknúť **Ochrana** v OWA.</span><span class="sxs-lookup"><span data-stu-id="83fc6-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="83fc6-109">To sa vzťahuje povolenie "Do not forward".</span><span class="sxs-lookup"><span data-stu-id="83fc6-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="83fc6-110">Kliknite na položku **zmeniť povolenie** a vyberte voľbu **Zašifrovať** iba šifrovanie správy.</span><span class="sxs-lookup"><span data-stu-id="83fc6-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="83fc6-111">Ak používate **klienta Outlook**: odoslať šifrovanú správu z programu Outlook 2013 alebo 2016 alebo Outlook 2016 for Mac, vyberte polo¾ku **Voåby** > **povolenia**a potom vyberte možnosť ochrany, ktoré potrebujete.</span><span class="sxs-lookup"><span data-stu-id="83fc6-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="83fc6-112">Na **automatické šifrovanie všetkých e-mailov** odoslané do určitých príjemcov alebo externej partnerskej organizácie, musíte vytvoriť pravidlo prenosu pošty toku v Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="83fc6-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="83fc6-113">Podrobné pokyny sú uvedené v [tomto článku technickej podpory](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="83fc6-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

