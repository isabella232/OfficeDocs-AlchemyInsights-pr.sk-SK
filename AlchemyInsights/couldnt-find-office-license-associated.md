---
title: Oprava aplikácií Microsoft 365 nenašiel priradené správy o licenciách balíka Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747710"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Oprava aplikácií Microsoft 365 sa nepodarilo nájsť priradenú licenciu na Office

Ak sa zobrazí toto hlásenie, vyskúšajte tieto kroky:

1. Skontrolujte bránu firewall, antivírusový softvér a nastavenia servera proxy a potvrďte, že neblokujú prístup na internet k aplikáciám Microsoft 365. Pozrite si tému [URL adresy a rozsahy IP adries pre Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Odstránenie a opätovné [Priradenie licencie na Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pre príslušného používateľa. 
3. Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.
4. Prejdite na položky Nastavenie systému Windows > **kontá**  >  **e-mailové & kontá**a odstráňte všetky pracovné kontá okrem príslušného konta.
5. Prejdite na položky Nastavenie systému Windows > prístup k **kontám**v  >  **práci alebo škole**a odpojte všetky pracovné kontá okrem príslušného konta.
6. Obnovte stav aktivácie balíka Office. [Zistite, ako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)na to.
7. [Prihláste](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sa pomocou príslušného používateľského konta.

Ďalšie riešenia na riešenie problémov nájdete v téme chyby týkajúce sa produktu bez platnej [licencie a aktivácie balíka Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).