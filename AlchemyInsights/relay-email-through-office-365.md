---
title: Prenos e-mailov prostredníctvom služieb Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117998"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="d4800-102">Nastavenie multifunkčného zariadenia alebo aplikácie na odosielanie e-mailov</span><span class="sxs-lookup"><span data-stu-id="d4800-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="d4800-103">Ak chcete získať informácie o možnostiach a postupoch, pozrite si tému [Nastavenie multifunkčného zariadenia alebo aplikácie na odosielanie e-mailov pomocou služieb Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="d4800-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="d4800-104">Ak máte zariadenie alebo aplikáciu, ktorá nedávno prestala fungovať, najbežnejšie problémy sú:</span><span class="sxs-lookup"><span data-stu-id="d4800-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="d4800-105">**Chyby týkajúce sa overovania pri používaní odosielania klienta SMTP Auth** Nedávno sme vykonali niekoľko zmien týkajúcich sa spôsobu overovania SMTP.</span><span class="sxs-lookup"><span data-stu-id="d4800-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="d4800-106">Ďalšie informácie o riešení problémov nájdete v časti Neúspešné overovanie v téme Riešenie problémov s tlačiarňami, skenermi a [aplikáciami LOB,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)ktoré odosielali e-maily pomocou služby Microsoft 365 alebo Office 365.</span><span class="sxs-lookup"><span data-stu-id="d4800-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="d4800-107">**Súhlasím iba s verziou TLS 1.2 počas zabezpečeného pripojenia k Office 365** Ak používate zabezpečené pripojenie (TLS), uistite sa, že vaše aplikačné zariadenie podporuje PROTOKOL TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="d4800-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="d4800-108">Ďalšie informácie nájdete v téme [Príprava na TLS 1.2 v téme Office 365 a Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="d4800-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="d4800-109">Ďalšie problémy a riešenia nájdete v téme Riešenie problémov s tlačiarňami, skenermi a [aplikáciami LOB,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)ktoré odosielali e-maily pomocou Microsoft 365 alebo Office 365.</span><span class="sxs-lookup"><span data-stu-id="d4800-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="d4800-110">Ak chcete zobraziť ovplyvnené zariadenia, prejdite na [zostavu klienta overovania protokolu SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d4800-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="d4800-111">**Poznámka:** Exchange Online sa nevyhodí scenárom hromadnej korešpondencie.</span><span class="sxs-lookup"><span data-stu-id="d4800-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="d4800-112">Ak chcete odosielať hromadné komerčné e-maily (napríklad zákaznícke bulletiny), mali by ste použiť poskytovateľov tretích strán, ktorí sa v týchto službách špecializovaní na ne zídu.</span><span class="sxs-lookup"><span data-stu-id="d4800-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
