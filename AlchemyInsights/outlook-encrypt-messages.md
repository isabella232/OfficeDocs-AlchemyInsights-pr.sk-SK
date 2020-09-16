---
title: S/MIME v Outlooku na webe
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772313"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="ae46a-102">Šifrovanie e-mailových správ v Outlooku</span><span class="sxs-lookup"><span data-stu-id="ae46a-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="ae46a-103">Šifrovanie správ v Microsoft 365 je postavené na lokalite Microsoft Azure Rights Management (Azure RMS), ktorá je súčasťou ochrany informácií Azure.</span><span class="sxs-lookup"><span data-stu-id="ae46a-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="ae46a-104">Ak vaše predplatné zahŕňa Azure Rights Management alebo Azure Information Protection, **nemusíte vykonávať žiadne akcie na manuálne zapnutie alebo aktiváciu** služby správy prístupových práv.</span><span class="sxs-lookup"><span data-stu-id="ae46a-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="ae46a-105">Na základe pripomienok od zákazníkov už nebudeme povoľovať pravidlá toku pošty v Exchangei, aby sa predvolene automaticky zašifroval odchádzajúci e-mail obsahujúci určitý typ citlivých informácií v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="ae46a-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="ae46a-106">Namiesto toho poskytujeme podrobné pokyny o tom, ako môžete tak urobiť sami.</span><span class="sxs-lookup"><span data-stu-id="ae46a-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="ae46a-107">Ďalšie podrobnosti o tom, ako vytvoriť pravidlo prenosu na šifrovanie citlivých informácií, nájdete v [tomto článku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="ae46a-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="ae46a-108">Ak používate Outlook na webe (predtým **OWA**): pri vytváraní e-mailovej správy jednoducho kliknite na položku **zabezpečiť** v aplikácii OWA.</span><span class="sxs-lookup"><span data-stu-id="ae46a-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="ae46a-109">Použije sa povolenie na preposielanie ďalej.</span><span class="sxs-lookup"><span data-stu-id="ae46a-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="ae46a-110">Kliknite na položku **zmeniť povolenie** a výberom položky **šifrovať** zašifrujete len správu.</span><span class="sxs-lookup"><span data-stu-id="ae46a-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="ae46a-111">Ak používate **klienta Outlook**: Ak chcete odoslať šifrovanú správu z Outlooku 2013 alebo 2016 alebo Outlooku 2016 pre Mac **Options**, vyberte položku  >  **povolenia**pre možnosti a potom vyberte požadovanú možnosť ochrany.</span><span class="sxs-lookup"><span data-stu-id="ae46a-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="ae46a-112">Ak chcete **automaticky šifrovať všetky e-maily** odoslané určitým príjemcom alebo externým partnerským organizáciám, musíte vytvoriť pravidlo prenosu toku pošty v centre spravovania pre Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae46a-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="ae46a-113">Podrobné pokyny sú uvedené v [tomto článku technickej podpory](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="ae46a-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

