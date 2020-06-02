---
title: S/MIME v Outlooku na webe
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511523"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="96157-102">Šifrovanie e-mailových správ v programe Outlook</span><span class="sxs-lookup"><span data-stu-id="96157-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="96157-103">Microsoft 365 šifrovanie správ je postavený na Microsoft Azure Rights Management (Azure RMS), ktorý je súčasťou Azure information protection.</span><span class="sxs-lookup"><span data-stu-id="96157-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="96157-104">Ak vaše predplatné zahŕňa Azure Rights Management alebo Azure information protection, **nie je potrebné vykonať žiadne akcie manuálne zapnúť alebo aktivovať** službu správy prístupových práv.</span><span class="sxs-lookup"><span data-stu-id="96157-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="96157-105">Na základe spätnej väzby od zákazníkov už nebudeme povoľovať pravidlá toku pošty servera Exchange na automatické šifrovanie odchádzajúcich e-mailov obsahujúcich určitý typ citlivých informácií vo vašom nájomníkovi v predvolenom nastavení.</span><span class="sxs-lookup"><span data-stu-id="96157-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="96157-106">Namiesto toho poskytujeme podrobné pokyny o tom, ako to môžete urobiť sami.</span><span class="sxs-lookup"><span data-stu-id="96157-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="96157-107">Ďalšie podrobnosti o tom, ako vytvoriť pravidlo prenosu na šifrovanie citlivých informácií, nájdete v [tomto článku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="96157-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="96157-108">Ak používate program Outlook na webe (predtým **OWA):** Pri vytváraní e-mailovej správy, jednoducho kliknite na tlačidlo **Chrániť** v OWA.</span><span class="sxs-lookup"><span data-stu-id="96157-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="96157-109">To to bude platiť "Neposielať ďalej" povolenie.</span><span class="sxs-lookup"><span data-stu-id="96157-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="96157-110">Ak chcete správu zašifrovať, kliknite na položku **Zmeniť povolenie** a výberom položky **Zašifrovať** iba správu.</span><span class="sxs-lookup"><span data-stu-id="96157-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="96157-111">Ak používate **klienta Programu Outlook**: Ak chcete odoslať zašifrovanú správu z Outlooku 2013 alebo 2016 alebo Outlooku 2016 for Mac, vyberte položku Povolenia **Options**  >  **možností**a potom vyberte požadovanú možnosť ochrany.</span><span class="sxs-lookup"><span data-stu-id="96157-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="96157-112">Ak chcete **automaticky šifrovať všetky e-maily** odoslané určitým príjemcom alebo externým partnerským organizáciám, musíte v Centre spravovania pre Exchange vytvoriť pravidlo prenosu toku pošty.</span><span class="sxs-lookup"><span data-stu-id="96157-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="96157-113">Podrobné pokyny sú uvedené v [tomto článku podpory](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="96157-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

