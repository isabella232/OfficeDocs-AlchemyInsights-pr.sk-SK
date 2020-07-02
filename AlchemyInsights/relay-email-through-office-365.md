---
title: Prenos e-mailov prostredníctvom služieb Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023474"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="2c888-102">Nastavenie multifunkčného zariadenia alebo aplikácie na odosielanie e-mailov</span><span class="sxs-lookup"><span data-stu-id="2c888-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="2c888-103">Ak chcete získať informácie o možnostiach a postupoch, pozrite si tému [Nastavenie multifunkčného zariadenia alebo aplikácie na odosielanie e-mailov pomocou služieb Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="2c888-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="2c888-104">**Poznámka:** Ak máte zariadenie alebo aplikáciu, ktorá nedávno prestala fungovať, upozorňujeme, že nedávno sme podľa plánu začali [vypínať 3DES šifrovanie](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="2c888-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="2c888-105">Ak chcete zobraziť ovplyvnené zariadenia, prejdite na [zostavu klienta overovania protokolu SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="2c888-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="2c888-106">Bežné chyby môžu byť tohto typu: zlyhanie/chyba overenia, zlyhanie/chyba TLS, chyba algoritmu šifrovania, nezhoda algoritmov alebo chyba pripojenia.</span><span class="sxs-lookup"><span data-stu-id="2c888-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="2c888-107">Riešenie problému:</span><span class="sxs-lookup"><span data-stu-id="2c888-107">To resolve the issue:</span></span>

 - <span data-ttu-id="2c888-108">**Windows Server 2003 IIS SMTP už nebude fungovať – vyžaduje sa novšia verzia Windowsu.**</span><span class="sxs-lookup"><span data-stu-id="2c888-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="2c888-109">Obráťte sa na dodávateľa aplikácie alebo zariadenia a zistite, či sa podporuje moderné šifrovanie alebo či je k dispozícii aktualizácia.</span><span class="sxs-lookup"><span data-stu-id="2c888-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
