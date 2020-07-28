---
title: Nie je nastavený certifikát push apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440011"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Nie je nastavený certifikát push apple MDM

Certifikát push mdm apple mdm (známy aj ako certifikát služby APNS (Apple Push Notification Service) nebol nakonfigurovaný pre vaše predplatné. Bez nakonfigurovaného push certifikátu Apple MDM sa nedarí zaregistrovať a spravovať zariadenia so systémom iOS a Mac OS. Po pridaní certifikátu do služby Intune môžu používatelia nainštalovať aplikáciu Portál spoločnosti na registráciu svojich zariadení so systémom iOS.

1. Vyberte **"Súhlasím".** spoločnosti Microsoft povolenie na odosielanie údajov spoločnosti Apple.

2. Vyberte **položku Download your CSR** the Intune certificate signing request required to create a Apple MDM push certificate. Súbor sa používa na vyžiadanie certifikátu vzťahu dôveryhodnosti z portálu Apple Push Certificates Portal.

3. Výberom **položky Create your MDM push Certificate (Vytvoriť certifikát push MDM)** prejdite na portál Apple Push Certificates Portal. Prihláste sa pomocou svojho firemného účtu Apple ID a vyberte **položku Vytvoriť certifikát**. Vyberte **položku Vybrať súbor**, vyhľadajte súbor žiadosti o podpisovanie certifikátov a potom vyberte položku **Odovzdať**. Na stránke Potvrdenie vyberte **položku Prevziať,** ak chcete prevziať súbor certifikátu (.pem) a súbor uložte lokálne.
 
**Poznámka:** Certifikát je priradený k účtu Apple ID, ktorý sa používa na jeho vytvorenie. Ako osvedčený postup použite na správu úloh apple ID spoločnosti a uistite sa, že poštovú schránku monitoruje viac ako jedna osoba alebo pomocou distribučného zoznamu. Nikdy nepoužívajte osobný účet Apple ID. Na obnovenie certifikátu Apple Push každých 12 mesiacov použite rovnaký účet Apple ID.
 
4. Zadajte účet Apple ID použitý na vytvorenie certifikátu push Apple MDM. Zaznamenajte túto identifikáciu ako pripomenutie, keď potrebujete certifikát obnoviť.

5. Prejdite do súboru certifikátu (.pem), vyberte položku **Otvoriť a**potom vyberte položku **Odovzdať**. Pomocou push certifikátu môže intune zaregistrovať a spravovať zariadenia Apple.