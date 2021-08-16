---
title: Teams chyby 4c7
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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049323"
---
# <a name="4c7-error-in-microsoft-teams"></a>Chyba 4c7 v Microsoft Teams

Táto chyba sa vyskytuje, Microsoft Teams vyžaduje overovanie formulárov. Keď nasadzujete Active Directory Federation Services (ADFS), overovanie formulárov nie je predvolene povolené pre intranet. Ak Windows integrované overovanie zlyhá, zobrazí sa výzva na prihlásenie pomocou overenia formulárov.

Ak chcete tento problém vyriešiť, povoľte overovanie formulárov pomocou modulu Microsoft Management Console (MMC) služby ADFS v počítači, ktorý obsahuje lokálnu kópiu služby Active Directory. Postupujte takto: 

1. Na navigačnej table prejdite na položku **Politiky overovania.**
2. V **časti Akcie** na table s podrobnosťami vyberte položku Upraviť globálne primárne **overovanie**.
3. Na karte **Intranet** vyberte položku **Overovanie formulárov.**
4. Vyberte **tlačidlo OK** (alebo **Použiť**).