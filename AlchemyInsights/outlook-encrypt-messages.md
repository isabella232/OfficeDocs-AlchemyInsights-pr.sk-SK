---
title: S/MIME v programe Outlook na webe
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764887"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="181c0-102">Šifrovať e-mailové správy v programe Outlook</span><span class="sxs-lookup"><span data-stu-id="181c0-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="181c0-103">Microsoft 365 šifrovanie správ je postavená na Microsoft Azure Rights Management (Azure RMS), ktorý je súčasťou Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="181c0-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="181c0-104">Ak vaše predplatné zahŕňa Azure Rights Management alebo Azure ochranu informácií, nemusíte **podniknúť žiadne kroky na manuálne povolenie alebo aktiváciu** služby správy prístupových práv.</span><span class="sxs-lookup"><span data-stu-id="181c0-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="181c0-105">Na základe spätnej väzby od zákazníkov už nebudeme umožňovať pravidlá toku poštových služieb Exchange, aby sa automaticky zašifrovali odchádzajúce e-maily obsahujúce určitý typ citlivých informácií v nájomníkovi predvolene.</span><span class="sxs-lookup"><span data-stu-id="181c0-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="181c0-106">Namiesto toho poskytujeme podrobné pokyny, ako to môžete urobiť sami.</span><span class="sxs-lookup"><span data-stu-id="181c0-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="181c0-107">Ďalšie informácie o tom, ako vytvoriť pravidlo prenosu na zašifrovanie citlivých informácií, nájdete [v tomto článku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="181c0-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="181c0-108">Ak používate program Outlook na webe (predtým **OWA**): pri vytváraní e-mailovej správy, jednoducho kliknite na tlačidlo **chrániť** v aplikácii OWA.</span><span class="sxs-lookup"><span data-stu-id="181c0-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="181c0-109">Toto bude platiť povolenie "Neposielať ďalej".</span><span class="sxs-lookup"><span data-stu-id="181c0-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="181c0-110">Kliknite na tlačidlo **zmeniť povolenie** a vyberte **Zašifrovať** len zašifrovať správy.</span><span class="sxs-lookup"><span data-stu-id="181c0-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="181c0-111">Ak používate **klienta Outlook**: Ak chcete odoslať zašifrovanú správu z programu Outlook 2013 alebo 2016, alebo Outlook 2016 pre Mac, vyberte **Možnosti** > **povolenia**, potom vyberte možnosť ochrany, ktorú potrebujete.</span><span class="sxs-lookup"><span data-stu-id="181c0-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="181c0-112">Ak chcete **automaticky zašifrovať všetky e-maily** odoslané určitým príjemcom alebo externým partnerským organizáciám, musíte v stredisku Exchange Admin Center vytvoriť pravidlo prenosu pošty.</span><span class="sxs-lookup"><span data-stu-id="181c0-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="181c0-113">Podrobné inštrukcie sú uvedené v [tomto článku podpory](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="181c0-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

