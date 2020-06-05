---
title: Aktivácia Problém - Sme schopní sa pripojiť práve teraz
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581890"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Oprava správy aplikácie Microsoft 365 "Momentálne sa nedá pripojiť"

Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúci postup:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy, aby ste potvrdili, že neblokujú prístup na Internet k aplikáciám Microsoft 365. Pozrite [si webové adresy a rozsahy adries IP od spoločnosti Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Prejdite do ponuky **Spustiť**  >  **a**zadajte **text services.msc**. Uistite sa, že všetky nasledujúce služby sú spustené:
    - Automatické nastavenie pripojených sieťových zariadení
    - Služba zoznam siete
    - Povedomie o sieťovom umiestnení
    - Denník udalostí systému Windows

Ak nie je spustená nie ktorá z týchto služieb, skúste ju spustiť. Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s právami správcu:

**Sfc / scannow SFC / scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti ["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" chyba pri aktivácii balíka Office od spoločnosti Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).