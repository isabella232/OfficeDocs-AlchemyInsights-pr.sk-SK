---
title: Konfigurovať DLP koncového bodu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402453"
---
# <a name="configure-endpoint-dlp"></a>Konfigurovať DLP koncového bodu

Microsoft Endpoint DLP umožňuje rozšíriť ochranu pred únikom údajov a možnosti monitorovania na citlivé informácie v zariadeniach s Windowsom 10. Po zaradení zariadení do správy zariadení môžete vytvoriť politiky DLP na vynútenie ochranných akcií pre položky. Prieskumník aktivít možno použiť na monitorovanie citlivých položiek v aktivite. Ďalšie informácie nájdete v téme [Zaradenie zariadení do správy zariadení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Ak chcete začať pracovať s DLP koncového bodu:

- Skontrolujte, či máte príslušné licencie na jednotku SKU/predplatné. Ďalšie informácie nájdete v téme [Licencie na jednotku SKU/predplatné](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Skontrolujte povolenia potrebné na povolenie správy zariadení, prístup na stránku zaradenia alebo zapnutie alebo vypnutie monitorovania zariadenia. Ďalšie informácie nájdete v téme [Povolenia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Zaraďte zariadenia do Správy zariadení pomocou postupu na zaradenie zariadení. Ak v časti **Nastavenia** dodržiavania súladu pre M365 chýba možnosť Zaradenie zariadenia (ukážka), skontrolujte, či máte príslušnú licenciu a povolenia uvedené vyššie. Ďalšie informácie nájdete v téme [Zaradenie zariadení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Vytvorte politiky DLP na ochranu citlivých položiek. Informácie nájdete v téme [Scenáre politiky DLP koncového bodu](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Ďalšie informácie o nástroji Microsoft Endpoint DLP nájdete v téme [Informácie o ochrane pred únikom údajov v koncovom bode pre Microsoft 365 (ukážka)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Dôležité kroky na zhromažďovanie údajov, ak je potrebná podpora:**

1. Stiahnite verziu preview diagnostického nástroja MDATP Client Analyzer z lokality [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Spustite nástroj ako správca v okne cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Po zobrazení výzvy „Zadajte počet minút na zhromažďovanie sledovania:“ zadajte počet minút, ktoré sú potrebné na spustenie scenára
5. Spustite scenár

Zhromaždite výstup súboru ZIP, ktorý poskytnete agentovi podpory.
