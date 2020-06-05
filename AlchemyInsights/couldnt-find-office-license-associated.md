---
title: Oprava aplikácií microsoft 365 Nepodarilo sa nájsť office licencie priradené správy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580456"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Oprava správy aplikácie Microsoft 365 "Nepodarilo sa nájsť priradené licencie balíka Office"

Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúci postup:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy, aby ste potvrdili, že neblokujú prístup na Internet k aplikáciám Microsoft 365. Pozrite si [článok Adresy URL a rozsahy adries IP od spoločnosti Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Odstráňte a [znova priraďte licenciu balíka Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pre príslušného používateľa. 
3. Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z existujúcich používateľských kont.
4. Prejdite do časti Nastavenie systému Windows > **kontá**  >  **E-mailové & kontá**a odstráňte všetky pracovné kontá okrem príslušného konta.
5. Prejdite do časti Nastavenie systému Windows > **kontá**  >  **Prístup k práci alebo škole**a odpojte všetky pracovné kontá okrem príslušného konta.
6. Obnovte stav aktivácie balíka Office. [Prečítajte si, ako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Prihláste sa](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou príslušného používateľského konta.

Ďalšie riešenia problémov nájdete v téme [Chyby produktu bez platnej licencie a aktivácie v balíku Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).