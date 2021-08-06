---
title: Pracovný deň pre poskytovanie používateľov služby AD prejde do karantény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036507"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Pracovný deň pre poskytovanie používateľov služby AD prejde do karantény

**Pracovný deň pre poskytovanie používateľov služby AD prejde do stavu karantény a v AD sa vytvárajú všetci používatelia**

Pracovný deň úlohy poskytovania používateľov služby AD prešlo do stavu karantény a denníky auditu zobrazujú udalosti zlyhania exportu s chybým hlásením **Chyba: OperationsError-SvcErr: Vyskytla sa chyba operácie. Pre adresárovú službu nie je nakonfigurovaný žiaden nadriadený odkaz. Adresárová služba preto nemôže vydať odporúčania k objektom mimo tejto doménovej ulice.** Táto chyba sa zvyčajne zobrazí, ak objekt OU kontajnera služby Active Directory nie je nastavený správne alebo ak sa vyskytuje problém s mapovaním výrazov použitým pre **nadradenýZozákaznýNázov.**

Skontrolujte preklepy v poli **Predvolená OU** pre parameter Noví používatelia. Presvedčte sa, či už v AD existuje zadaná OU. Ak v mapovaní atribútov používate **atribút parentDistinguishedName,** uistite sa, že sa vždy vyhodnotí ako známy kontajner v rámci domény AD. Skontrolujte vygenerovanú hodnotu v udalosti Exportovať v denníkoch auditu.

Ďalšie podrobnosti o konfigurácii pracovného dňa na automatické poskytovanie údajov nájdete v [kurze: Konfigurácia pracovného dňa pre automatické poskytovanie služieb používateľom.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

