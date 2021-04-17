---
title: Oprava hlásenia o oprave aplikácií služby Microsoft 365 Nepodarilo sa nájsť licencie balíka Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816503"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Oprava hlásenia o oprave aplikácií služby Microsoft 365 "Nepodarilo sa nájsť licencie balíka Office priradené"

Ak sa zobrazí toto hlásenie, skúste toto:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet k aplikáciám služby Microsoft 365. Pozrite si časť URL adresy a rozsahy IP adries v [Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Odobrať [a zmeniť priradenie licencie na Office pre](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) príslušného používateľa. 
3. Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.
4. Prejdite na nastavenia Windowsu > **Kontá**  >  **e-& kontá a** odstráňte všetky pracovné kontá okrem príslušného konta.
5. Prejdite na nastavenia Windowsu > **Kontá**  >  **prístup k pracovnému alebo školskému** a odpojte všetky pracovné kontá okrem príslušného konta.
6. Obnovte stav aktivácie balíka Office. [Zistite, ako na to.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Prihláste sa](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou príslušného používateľského konta.

Ďalšie riešenia problémov nájdete v téme Chyba [produktu bez licencie a chyba aktivácie v Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)