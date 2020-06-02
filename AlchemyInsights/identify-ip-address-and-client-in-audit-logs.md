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
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508931"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifikácia adresy IP a klienta v denníkoch auditu

Adresa IP, ktorá zodpovedá aktivite používateľa alebo správcu služby Microsoft 365, sa zobrazuje v denníkoch auditu. Informácie o klientovi sa tiež zaznamená. Tu sú kroky na identifikáciu týchto informácií

1. Prihláste sa do Centra [& zabezpečenia spoločnosti Microsoft 365](https://protection.office.com/).

2. Prejdite na stránku **vyhľadávania**  >  **v denníku auditu.**

   Ak máte záujem o konkrétnu aktivitu, vyberte ju zo zoznamu **Aktivity.** Ak nie, všetky aktivity sa vrátia pre vybratého používateľa (predvolené nastavenie).

   **Poznámka:** Niektoré činnosti nemusia byť k dispozícii v menu **Aktivity;** Tieto položky auditu sa však vrátia, ak je vybratá možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené nastavenie).

3. Zadajte meno používateľa do poľa **Používatelia,** vyberte príslušný rozsah dátumov pre aktivitu a potom kliknite na tlačidlo **Hľadať**.

Vo výsledkoch sa na table s výsledkami zobrazuje adresa IP pre danú aktivitu. Vyberte záznam auditu a zobrazia sa podrobné informácie v rozbaľovacom zozname **Podrobnosti** (napríklad Klient, Používateľ, ktorý vykonal akciu atď.).

Ďalšie informácie sa nachádzajú v téme [Vyhľadanie adresy IP počítača používaného na prístup k ohrozenému kontu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
