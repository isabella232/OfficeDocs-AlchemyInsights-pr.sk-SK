---
title: Pracovný deň na poskytovanie AD používateľov ide do stavu karantény
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482903"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Pracovný deň na poskytovanie AD používateľov ide do stavu karantény

**Pracovný deň na poskytovanie AD používateľov prejde do stavu karantény a v službe AD sa nevytvára žiaden používateľ**

Pracovný deň s poskytnutím úlohy AD user v karanténe a denníky auditu zobrazujú udalosti zlyhania exportu s chybovým hlásením **chyba: OperationsError-SvcErr: Vyskytla sa chyba operácie. Pre adresárovú službu nebol nakonfigurovaný žiadny nadriadený odkaz. Adresárová služba preto nedokáže vydať odporúčania na objekty mimo tohto lesa**. Táto chyba sa zvyčajne zobrazuje v prípade, že kontajner služby Active Directory nie je nastavený správne alebo ak sa vyskytnú problémy s priradením výrazov, ktoré sa používajú pre **parentDistinguishedName**.

Skontrolujte predvolený parameter OU pre **nových používateľov** pre preklepy. Uistite sa, že určitá OU už v REKLAMe existuje. Ak v priradení atribútov používate **parentDistinguishedName** , uistite sa, že sa vždy vyhodnotí v rámci reklamnej domény známym kontajnerom. Ak chcete zobraziť vygenerovanú hodnotu, pozrite si udalosť exportu v denníkoch auditu.

Ďalšie informácie o konfigurácii pracovného dňa na automatické poskytovanie informácií nájdete v téme [kurz: Konfigurácia pracovného dňa na automatické poskytovanie používateľov](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

