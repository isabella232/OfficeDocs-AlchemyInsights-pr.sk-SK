---
title: 2491 upozorniť na e-mailové správy z Phish doručené z dôvodu politiky prepísania nájomníka alebo používateľa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728626"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="dba21-102">Upozorniť na e-mailové správy z Phish doručené z dôvodu politiky prepísania nájomníka alebo používateľa</span><span class="sxs-lookup"><span data-stu-id="dba21-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="dba21-103">Na nájomníkov s licenciami na Office 365 ATP P1 a P2 boli prevzaté predvolené politiky upozornení s názvom Phish doručené z dôvodu prepísania nájomníka alebo používateľa.</span><span class="sxs-lookup"><span data-stu-id="dba21-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="dba21-104">Ak ste prijali toto upozornenie, tu sú uvedené kroky, ktoré je potrebné preskúmať:</span><span class="sxs-lookup"><span data-stu-id="dba21-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="dba21-105">V upozorňujúcej správe kliknite na položku **Zobraziť upozornenie** , čím prejdete na stránku **upozornenia** v centre zabezpečenia & dodržiavania súladu.</span><span class="sxs-lookup"><span data-stu-id="dba21-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="dba21-106">Vyberte upozornenie, aby sa zobrazila možnosť **Zobraziť zoznam správ** alebo **Zobraziť správy v Prieskumníkovi**.</span><span class="sxs-lookup"><span data-stu-id="dba21-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="dba21-107">Obe tieto možnosti sa donesú do podrobností o správe, ktorá obsahuje identifikáciu správy.</span><span class="sxs-lookup"><span data-stu-id="dba21-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="dba21-108">Všimnite si, že prepojenie na program Threat Explorer automaticky filtruje správy, ktoré zodpovedajú kritériám upozornenia.</span><span class="sxs-lookup"><span data-stu-id="dba21-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="dba21-109">Možno bude potrebné nastaviť filter dátumu v programe Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="dba21-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="dba21-110">Správa neoprávneného získavania údajov bola doručená z dôvodu manuálne nakonfigurovaného prepísania:</span><span class="sxs-lookup"><span data-stu-id="dba21-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="dba21-111">Povolený odosielateľ alebo doména, ktorú používateľ nastavil.</span><span class="sxs-lookup"><span data-stu-id="dba21-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="dba21-112">Povoleného odosielateľa alebo domény nastavenej správcom v politike ochrany pred nevyžiadanou poštou.</span><span class="sxs-lookup"><span data-stu-id="dba21-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="dba21-113">Povolená IP adresa v politike filtrovania pripojení.</span><span class="sxs-lookup"><span data-stu-id="dba21-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="dba21-114">Pravidlo toku pošty (označuje sa aj ako pravidlo prenosu), ktoré je nakonfigurované na povolenie správ v programe.</span><span class="sxs-lookup"><span data-stu-id="dba21-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="dba21-115">Ak sa domnievate, že správa bola nesprávne označená ako Phish, na odoslanie vzoriek správ do spoločnosti Microsoft použite [doplnok správa zostavy](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="dba21-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
