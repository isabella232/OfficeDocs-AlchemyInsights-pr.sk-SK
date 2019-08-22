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
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539044"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Určiť adresy IP a klient v denníkoch auditu

Adresu IP, ktorá zodpovedá činnosti Office 365 používateľa alebo správcu je uvedený v denníkoch auditu. Informácie o klientovi je tiež prihlásený. Tu sú kroky na identifikáciu takýchto informácií

1. Prihláste sa do [Centrum Office 365 zabezpečenia & súladu](https://protection.office.com/).

2. Prejdite na **vyhľadávanie** > stránka**vyhľadávanie denník auditu** .

   Ak máte záujem v konkrétnej činnosti, vyberte ho zo zoznamu **činností** . Ak nie, vrátia všetky aktivity pre vybratého používateľa (predvolené nastavenie).

   **Poznámka**: niektoré činnosti nemusia byť dostupné v menu **aktivity** ; však o audite položky budú vrátené Ak **Ukázať výsledky všetkých činností** je (predvolené nastavenie).

3. V poli **Používatelia** zadať užívateľské meno, vyberte príslušný rozsah dátumov pre aktivitu a kliknite na tlačidlo **Hľadať**.

Vo výsledkoch zobrazí adresu IP pre túto činnosť v table výsledky. Vyberte auditný záznam zobrazíte podrobné informácie v **Podrobnosti** Nadjazd (napríklad klient, používateľ, ktorý vykonáva akcie, atď.).

Ďalšie informácie nájdete v téme [Lokalizovanie adresu IP počítača používa na prístup k ohrozeným kontom](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
