---
title: 2491 Alert email messages from the 'Phish Delivered due to tenant or user override' policy
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544593"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="20b77-102">E-mailové správy s upozornením z politiky prepísania nájomníka alebo používateľa sa doručujú phish Delivered</span><span class="sxs-lookup"><span data-stu-id="20b77-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="20b77-103">Pre nájomníkov pomocou nástroja Microsoft Defender pre Office 365 P1 a P2 sa v nájomníkoch zaregistrovala predvolená politika upozornenia s názvom Phish Delivered due to tenant or user override (Prepísanie nájomníka alebo používateľa).</span><span class="sxs-lookup"><span data-stu-id="20b77-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="20b77-104">Ak ste dostali toto upozornenie, preskúmajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="20b77-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="20b77-105">V upozornení kliknite na položku **Zobraziť upozornenie** a prejdite na stránku **Upozornenia** v Centre zabezpečenia & súladu.</span><span class="sxs-lookup"><span data-stu-id="20b77-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="20b77-106">Ak chcete zobraziť možnosť Zobraziť zoznam správ alebo **Zobraziť správy v Prieskumníkovi,** **vyberte upozornenie.**</span><span class="sxs-lookup"><span data-stu-id="20b77-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="20b77-107">Pomocou oboch týchto možností sa môžete o tejto správe postarať o podrobnosti, ktoré obsahujú identifikáciu správy.</span><span class="sxs-lookup"><span data-stu-id="20b77-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="20b77-108">Všimnite si, že prepojenie Prieskumník hrozieb automaticky filtruje správy, ktoré spĺňajú kritériá upozornenia.</span><span class="sxs-lookup"><span data-stu-id="20b77-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="20b77-109">Možno budete musieť upraviť filter dátumu v Prieskumníkovi hrozieb.</span><span class="sxs-lookup"><span data-stu-id="20b77-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="20b77-110">Správa s cieľom neoprávneného získavania údajov sa doručila z dôvodu manuálne nakonfigurovaného prepísania:</span><span class="sxs-lookup"><span data-stu-id="20b77-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="20b77-111">Povolený odosielateľ alebo doména nastavená používateľom.</span><span class="sxs-lookup"><span data-stu-id="20b77-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="20b77-112">Povolený odosielateľ alebo doména nastavená správcom v politike ochrany pred nevyžiadanou poštou.</span><span class="sxs-lookup"><span data-stu-id="20b77-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="20b77-113">Povolená IP adresa v politike filtrovania pripojenia.</span><span class="sxs-lookup"><span data-stu-id="20b77-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="20b77-114">Pravidlo toku pošty (známe aj ako pravidlo prenosu), ktoré je nakonfigurované na povolenie správ.</span><span class="sxs-lookup"><span data-stu-id="20b77-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="20b77-115">Ak si myslíte, že správa bola nesprávne označená ako phish, použite doplnok Outlook [Report Message a](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) odošlite vzorky správ spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20b77-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
