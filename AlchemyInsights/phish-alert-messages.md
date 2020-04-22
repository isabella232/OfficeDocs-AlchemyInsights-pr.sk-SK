---
title: 2491 upozorňujúce e-mailové správy z "Phish dodané z dôvodu nájomcu alebo používateľ prepísať" politiky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758948"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="5b0ce-102">Upozorňujúce e-mailové správy z ' Phish dodané z dôvodu nájomcu alebo používateľ prepísať ' politika</span><span class="sxs-lookup"><span data-stu-id="5b0ce-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="5b0ce-103">Predvolená politika upozornenia s názvom "Phish dodané z dôvodu nájomcu alebo prepísať používateľa" bola vrátená nájomníkmi s Office 365 ATP P1 a P2 licencie.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="5b0ce-104">Ak ste dostali Toto upozornenie, tu sú kroky na vyšetrenie:</span><span class="sxs-lookup"><span data-stu-id="5b0ce-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="5b0ce-105">Z upozorňujúce hlásenie, kliknite na tlačidlo **Zobraziť upozornenie** prejdite na stránku **upozornenia** v zabezpečenie & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="5b0ce-106">Vyberte upozornenie, ak chcete zobraziť možnosť **zobrazenia zoznamu správ** alebo **Zobraziť správy v Prieskumníkovi**.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="5b0ce-107">Obe tieto možnosti sa dostanete na Podrobnosti správy, ktorá obsahuje ID správy.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="5b0ce-108">Všimnite si, že hrozba Explorer odkaz bude automaticky filtrovať správy, ktoré zodpovedajú výstražné kritériá.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="5b0ce-109">Možno bude potrebné upraviť filter dátumu v programe Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="5b0ce-110">Hlásenie neoprávneného získavania údajov bolo dodané z dôvodu manuálne nakonfigurovaného prepísania:</span><span class="sxs-lookup"><span data-stu-id="5b0ce-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="5b0ce-111">Povolený odosielateľ alebo doména nastavená používateľom.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="5b0ce-112">Povolený odosielateľ alebo doména nastavená správcom v politike anti-spam.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="5b0ce-113">Povolená adresa IP v politike filtra pripojenia.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="5b0ce-114">Pravidlo toku pošty (známe aj ako pravidlo prenosu), ktoré je nakonfigurované na povolenie správ.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="5b0ce-115">Ak sa domnievate, že správa bola nesprávne označená ako Phish, použite [doplnok](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) správy programu Outlook na odoslanie vzoriek správ spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5b0ce-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
