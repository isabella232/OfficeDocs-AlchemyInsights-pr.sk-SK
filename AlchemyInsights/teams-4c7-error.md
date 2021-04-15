---
title: Chyba aplikácie Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786684"
---
# <a name="4c7-error-in-microsoft-teams"></a>Chyba 4c7 v aplikácii Microsoft Teams

Táto chyba sa vyskytuje, pretože aplikácia Microsoft Teams vyžaduje overovanie formulárov. Keď nasadzujete Active Directory Federation Services (ADFS), overovanie formulárov nie je predvolene povolené pre intranet. Ak integrované overovanie systému Windows zlyhá, zobrazí sa výzva na prihlásenie pomocou overenia formulárov.

Ak chcete tento problém vyriešiť, povoľte overovanie formulárov pomocou modulu Microsoft Management Console (MMC) služby ADFS v počítači, ktorý obsahuje lokálnu kópiu služby Active Directory. Postupujte takto: 

1. Na navigačnej table prejdite na položku **Politiky overovania.**
2. V **časti Akcie** na table s podrobnosťami vyberte položku Upraviť globálne primárne **overovanie**.
3. Na karte **Intranet** vyberte položku **Overovanie formulárov.**
4. Vyberte **tlačidlo OK** (alebo **Použiť**).