---
title: Konfigurovanie šifrovania správ pre hybridné prostredie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747949"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="82e2c-102">Konfigurovanie šifrovania správ pre hybridné prostredie</span><span class="sxs-lookup"><span data-stu-id="82e2c-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="82e2c-103">V prípade hybridných prostredí Exchange môžu Lokálni používatelia odosielať šifrované e-maily pomocou šifrovania správ balíka Office (OME) iba v prípade, že je e-mail smerovaný prostredníctvom služby Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="82e2c-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="82e2c-104">Ak chcete šifrovať e-maily pomocou OME, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="82e2c-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="82e2c-105">Ak chcete nastaviť hybridné prostredie, použite [Sprievodcu konfiguráciou hybridného](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) nasadenia.</span><span class="sxs-lookup"><span data-stu-id="82e2c-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="82e2c-106">Na nastavenie šifrovania nie sú potrebné žiadne špeciálne kroky.</span><span class="sxs-lookup"><span data-stu-id="82e2c-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="82e2c-107">[Nastavte pravidlá toku pošty na šifrovanie](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) , ako by ste mali normálne.</span><span class="sxs-lookup"><span data-stu-id="82e2c-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


