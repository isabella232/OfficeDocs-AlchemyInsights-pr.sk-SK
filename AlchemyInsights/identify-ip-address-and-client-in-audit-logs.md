---
title: Určiť adresy IP a klient v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382968"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Určiť adresy IP a klient v denníkoch auditu

Adresu IP, ktorá zodpovedá činnosť používateľa alebo správcu sa zobrazí denníky auditu. Informácie o klientovi je tiež prihlásený. Tu sú kroky na identifikáciu takýchto informácií

1. Prihláste sa do [Centrum Office 365 zabezpečenia & súlad](https://protection.office.com/)

2. Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte **Vyhľadávanie denník auditu**.

   Ak máte záujem v konkrétnej činnosti, vyberte ho zo zoznamu **činností** . Ak nie, vrátia všetky aktivity pre vybratého používateľa (predvolené nastavenie).

   **Poznámka**: niektoré činnosti nemusia byť dostupné v menu **aktivity** ; však o audite položky budú vrátené Ak **Ukázať výsledky všetkých činností** je (predvolené nastavenie).

3. V poli **Používatelia** zadať užívateľské meno, vyberte príslušný rozsah dátumov pre aktivitu a kliknite na tlačidlo **Hľadať**.

Vo výsledkoch zobrazí adresu IP pre túto činnosť v table výsledky. Vyberte auditný záznam zobrazíte podrobné informácie v **Podrobnosti** Nadjazd (napríklad klient, používateľ, ktorý vykonáva akcie, atď.).

Ďalšie informácie nájdete v téme [Lokalizovanie adresu IP počítača používa na prístup k ohrozeným kontom](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
