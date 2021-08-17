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
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887515"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifikácia IP adresy a klienta v denníkoch auditu

IP adresa, ktorá zodpovedá aktivite používateľa Microsoft 365 alebo správcu, sa zobrazí v denníkoch auditu. Zapíšu sa aj informácie o klientovi. Tu je postup na identifikáciu takýchto informácií

1. Prihláste sa do [Centra Microsoft 365 dodržiavania súladu.](https://protection.office.com/)

2. Prejdite na stránku **vyhľadávania denníka**  >  **auditu vyhľadávania.**

   Ak máte záujem o konkrétnu aktivitu, vyberte ju v **zozname** Aktivity. Ak nie, vrátia sa všetky aktivity vybratého používateľa (predvolené nastavenie).

   **Poznámka:** Niektoré aktivity nemusia byť v **ponuke Aktivity k** dispozícii. Tieto položky auditu sa však vrátia, ak **vyberiete** položku Zobraziť výsledky pre všetky aktivity (predvolené nastavenie).

3. Zadajte meno používateľa do **poľa Používatelia,** vyberte príslušný rozsah dátumov aktivity a potom kliknite na položku **Hľadať**.

Vo výsledkoch môžete zobraziť IP adresu pre túto aktivitu na table výsledkov. Výberom záznamu auditu zobrazte  podrobné informácie na letáku Podrobnosti (napríklad Klient, Používateľ, ktorý vykonal akciu atď.).

Ďalšie informácie nájdete v téme [Vyhľadanie IP adresy počítača používaných na prístup k zneužitemu kontu.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
