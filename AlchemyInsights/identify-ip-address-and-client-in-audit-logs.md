---
title: Identifikácia adresy IP a klienta v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716403"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifikácia adresy IP a klienta v denníkoch auditu

Adresa IP, ktorá zodpovedá aktivite používateľa alebo správcu spoločnosti Microsoft 365, sa zobrazí v denníkoch auditu. Informácie o klientovi je tiež prihlásený. Tu sú kroky na identifikáciu týchto informácií

1. Prihláste sa do [Microsoft 365 Security & centrum súladu](https://protection.office.com/).

2. Prejdite na stránku vyhľadávania**denníka auditu** **vyhľadávania** > .

   Ak máte záujem o konkrétnu aktivitu, vyberte ju zo zoznamu **aktivity** . Ak nie, všetky aktivity sa vrátia pre vybratého používateľa (predvolené nastavenie).

   **Poznámka**: niektoré aktivity nemusia byť k dispozícii v ponuke **aktivity** ; Tieto položky auditu sa však vrátia, ak je vybratá možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené nastavenie).

3. Zadajte meno používateľa v poli **Používatelia** , vyberte príslušný rozsah dátumov pre aktivitu a potom kliknite na tlačidlo **Hľadať**.

Vo výsledkoch môžete vidieť adresu IP danej aktivity na table s výsledkami. Vyberte záznam auditu a zobrazia sa podrobné informácie v rozbaľovacom zozname **Podrobnosti** (napríklad klient, používateľ, ktorý vykonal akciu atď.).

Ďalšie informácie nájdete v téme [vyhľadanie adresy IP počítača používaného na prístup k ohrozeným účtom](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
