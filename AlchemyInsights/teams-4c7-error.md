---
title: Chyba aplikácie teams 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700218"
---
# <a name="4c7-error-in-microsoft-teams"></a>chyba 4c7 v aplikácii Microsoft teams

Táto chyba sa vyskytuje, pretože Microsoft teams vyžaduje overovanie formulárov. Pri nasadzovaní služby Active Directory Federation Services (ADFS) (AD FS) nie je overovanie formulárov predvolene zapnuté pre intranet. Ak integrované overovanie systému Windows zlyhá, zobrazí sa výzva na prihlásenie pomocou overovania formulárov.

Ak chcete tento problém vyriešiť, povoľte overovanie formulárov pomocou modulu konzoly MMC (AD FS Microsoft Management Console) v počítači s lokálnou kópiou služby Active Directory. Postupujte takto: 

1. Na navigačnej table prejdite na položku **politiky overovania**.
2. V časti **akcie** na table s podrobnosťami vyberte položku **Upraviť globálne primárne overovanie**.
3. Na karte **intranet** vyberte položku **overovanie formulárov**.
4. Vyberte **tlačidlo OK** (alebo **použiť**).