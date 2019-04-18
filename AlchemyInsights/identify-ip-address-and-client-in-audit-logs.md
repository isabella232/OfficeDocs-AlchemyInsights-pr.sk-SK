---
title: Určiť adresy IP a klient v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909543"
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
