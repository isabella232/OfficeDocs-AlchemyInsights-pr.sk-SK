---
title: 2491 Upozornenie e-mailových správ z Phish doručiť pre nájomcu alebo užívateľa prepísať politiky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391516"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7a382-102">Upozornenie e-mailových správ z Phish doručiť pre nájomcu alebo užívateľa prepísať politiky</span><span class="sxs-lookup"><span data-stu-id="7a382-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7a382-103">Predvolené upozornenie politiku s názvom "Phish Delivered kvôli nájomcu alebo užívateľa prepísať" bola vyšiel nájomníkom s licencií balíka Office 365 ATP P1 a P2.</span><span class="sxs-lookup"><span data-stu-id="7a382-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7a382-104">Ak ste dostali túto výstrahu, tu sú kroky, aby vyšetrila:</span><span class="sxs-lookup"><span data-stu-id="7a382-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7a382-105">Výstražné hlásenie, kliknite na položku **Zobraziť upozornenia** prejdete na stránke **upozornenia** zabezpečenia & centrum súladu.</span><span class="sxs-lookup"><span data-stu-id="7a382-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7a382-106">Vyberte upozornenie vidieť možnosť **zobrazenia zoznamu správ** alebo **prezeranie správ v programe Prieskumník**.</span><span class="sxs-lookup"><span data-stu-id="7a382-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7a382-107">Obe tieto možnosti sa dostanete na údaje správy, ktorý zahŕňa správu ID.</span><span class="sxs-lookup"><span data-stu-id="7a382-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7a382-108">Všimnite si, že hrozba Explorer odkaz bude automaticky filtrovať správy, ktoré zodpovedajú varovania kritériá.</span><span class="sxs-lookup"><span data-stu-id="7a382-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7a382-109">Budete musieť nastaviť filter dátumu v Prieskumník hrozieb.</span><span class="sxs-lookup"><span data-stu-id="7a382-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7a382-110">Phishing správa bola doručená, pretože ručne konfigurované prepísať:</span><span class="sxs-lookup"><span data-stu-id="7a382-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7a382-111">Povolených odosielateľa alebo domény nastavená užívateľom.</span><span class="sxs-lookup"><span data-stu-id="7a382-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7a382-112">Povolených odosielateľa alebo doménu nastaviť admin anti-spam politiky.</span><span class="sxs-lookup"><span data-stu-id="7a382-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7a382-113">Povolené IP adresu pripojenia filtra politiky.</span><span class="sxs-lookup"><span data-stu-id="7a382-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7a382-114">Mail tok pravidlo (tiež známy ako pravidlo prenosu) je nakonfigurovaný tak, aby správy.</span><span class="sxs-lookup"><span data-stu-id="7a382-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7a382-115">Ak sa domnievate, že správa bola nesprávne označená ako phish, pomocou Outlook [doplnok hlásenie správy](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) predložiť správu vzorky do spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7a382-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
