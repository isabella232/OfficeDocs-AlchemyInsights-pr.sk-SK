---
title: Priradenia atribútov zabezpečenia používateľa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949895"
---
# <a name="user-provisioning-attribute-mapping"></a>Priradenia atribútov zabezpečenia používateľa

1. Ak chcete riešiť problémy so známym priradením atribútov, pozrite si tému [priradenia atribútov](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) poskytuje podporu pre poskytovanie používateľov na aplikácie SaaS tretích strán, ako je napríklad Salesforce, G Suite a ďalšie. Ak zapnete poskytovanie používateľov pre aplikáciu SaaS tretej strany, na portáli Azure sa riadia hodnoty atribútov prostredníctvom priradení atribútov. Informácie o prispôsobení predvolených priradení atribútov nájdete [v téme Prispôsobenie priradenia atribútov priradenia používateľov k aplikáciám SaaS v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Ďalšie informácie o zriaďovaní používateľov služby SaaS nájdete v téme [čo je poskytovanie automatizovaných používateľských aplikácií SaaS v službe Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Pri prispôsobovaní priradení atribútov pre poskytovanie používateľov sa môže stať, že sa atribút, ktorý chcete priradiť, nezobrazuje v zozname zdrojových atribútov. [Synchronizácia atribútu z lokálnej služby Active Directory do služby Azure AD na poskytovanie](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) v článku aplikácie vám ukáže, ako pridať chýbajúci atribút tak, že ho synchronizujete z lokálnej reklamy na Azure AD.
