---
title: Identifikácia IP adresy a klienta v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668325"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifikácia IP adresy a klienta v denníkoch auditu

IP adresa, ktorá zodpovedá aktivite používateľa alebo správcu Microsoft 365, sa zobrazí v denníkoch auditu. Informácie o klientovi sa tiež zaznamenávajú. Tu sú kroky na identifikáciu týchto informácií

1. Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/).

2. Prejdite na stránku **Search**  >  **vyhľadávania denníka auditu** vyhľadávania.

   Ak máte záujem o konkrétnu aktivitu, vyberte ju zo zoznamu **aktivity** . Ak nie, pre vybratého používateľa sa vrátia všetky aktivity (predvolené nastavenie).

   **Poznámka**: niektoré aktivity nemusia byť v ponuke **aktivity** k dispozícii. Tieto položky auditu sa však vrátia, ak je vybratá možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené nastavenie).

3. Zadajte meno používateľa v poli **Používatelia** , vyberte príslušný rozsah dátumov pre aktivitu a potom kliknite na položku **Hľadať**.

Vo výsledkoch môžete na table Výsledky Zobraziť IP adresu danej aktivity. Vyberte záznam auditu, aby sa zobrazili podrobné informácie v rozbaľovacom zozname **podrobností** (napríklad klient, používateľ, ktorý vykonal akciu atď.).

Ďalšie informácie nájdete v téme [Vyhľadanie IP adresy počítača, ktorý sa používa na prístup k ohrozenému kontu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
