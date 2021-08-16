---
title: Oprava Microsoft 365 hlásení o tom, že sa nepodarilo nájsť licencie balíka Office
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
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069619"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Oprava Microsoft 365 hlásení "Nepodarilo sa nájsť licencie balíka Office priradené"

Ak sa zobrazí toto hlásenie, skúste toto:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet Microsoft 365 aplikáciám. Pozrite [Microsoft 365 URL adresy a rozsahy IP adries.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Odobrať [a zmeniť priradenie Office pre](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) príslušného používateľa. 
3. Otvorte konto aplikácia Office [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z existujúcich používateľských kont.
4. Prejdite na Windows Nastavenia >   >  **e-mailové & kontá a** odstráňte všetky pracovné kontá okrem príslušného konta.
5. Prejdite na Windows Nastavenia > **prístup k** pracovným alebo  >  **školským kontám** a odpojte všetky pracovné kontá okrem príslušného konta.
6. Obnovte stav Office aktivácie produktov. [Zistite, ako na to.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Prihláste sa](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou príslušného používateľského konta.

Ďalšie riešenia problémov nájdete v téme [Chyba produktu bez licencie a chyba aktivácie v Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)