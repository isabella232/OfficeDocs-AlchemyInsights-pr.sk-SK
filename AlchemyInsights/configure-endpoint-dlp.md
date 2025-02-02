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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323933"
---
# <a name="configure-endpoint-dlp"></a>Konfigurovať DLP koncového bodu

Microsoft Endpoint DLP umožňuje rozšíriť ochranu pred únikom údajov a možnosti monitorovania na citlivé informácie v zariadeniach s Windowsom 10. Po zaradení zariadení do správy zariadení môžete vytvoriť politiky DLP na vynútenie ochranných akcií pre položky. Prieskumník aktivít možno použiť na monitorovanie citlivých položiek v aktivite. Ďalšie informácie nájdete v téme [Zaradenie zariadení do správy zariadení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Ak chcete začať pracovať s DLP koncového bodu:

- Skontrolujte, či máte príslušné licencie na jednotku SKU/predplatné. Ďalšie informácie nájdete v téme [Licencie na jednotku SKU/predplatné](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Skontrolujte povolenia potrebné na povolenie správy zariadení, prístup na stránku zaradenia alebo zapnutie alebo vypnutie monitorovania zariadenia. Ďalšie informácie nájdete v téme [Povolenia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Zaraďte zariadenia do Správy zariadení pomocou postupu na zaradenie zariadení. Ďalšie informácie nájdete v téme [Zaradenie zariadení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Vytvorte politiky DLP na ochranu citlivých položiek. Informácie nájdete v téme [Scenáre politiky DLP koncového bodu](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Ďalšie informácie o nástroji Microsoft Endpoint DLP nájdete v téme [Informácie o ochrane pred únikom údajov v koncovom bode pre Microsoft 365 (ukážka)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Dôležité kroky na zhromažďovanie údajov, ak je potrebná podpora:**

1. Stiahnuť [ukážku analýzy klienta MDATP.](https://aka.ms/betamdatpanalyzer)
1. Spustite nástroj ako správca v okne cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Po zobrazení **výzvy zadajte počet minút** na zhromaždenie sledovania: zadajte počet minút potrebných na spustenie scenára.
1. Spustite scenár.

Zhromaždite výstup súboru zip a dajte ho agentovi podpory.
