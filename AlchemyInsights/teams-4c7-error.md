---
title: Tímy 4c 7 chyba
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796360"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c 7 chyba v Microsoft teams

Táto chyba sa vyskytuje, pretože Microsoft teams vyžaduje overovanie formulárov. Pri nasadzovaní služby Active Directory Federation Services (AD FS), overovanie formulárov nie je povolená pre intranet predvolene. Ak Windows integrované overovanie zlyhá, sa zobrazí výzva na prihlásenie pomocou overovanie formulárov.

Ak chcete vyriešiť tento problém, povoľte overovanie formulárov pomocou modulu AD FS Microsoft Management Console (MMC) v počítači, ktorý má lokálnu kópiu služby Active Directory. Postupujte takto: 

1. Na navigačnej table prejdite na položku **politiky overovania**.
2. V časti **akcie** na table s podrobnosťami vyberte položku **Upraviť globálne primárne overovanie**.
3. Na karte **intranet** vyberte **overovanie formulárov**.
4. Vyberte položku **OK** (alebo **aplikovať**).