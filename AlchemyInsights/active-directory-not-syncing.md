---
title: Nesynchronizuje sa Active Directory
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822866"
---
# <a name="active-directory-not-syncing"></a>Nesynchronizuje sa Active Directory

Ak sa vám zobrazuje chyba synchronizácie, napríklad "žiadna nedávna synchronizácia" alebo ak si všimnete stav synchronizácie adresárov na portáli pre správcov balíka Office, zobrazí sa hlásenie Posledná synchronizácia pred viac ako 3 dňami, môže to byť preto, že AADConnect má na vykonanie synchronizácie nesprávne nastavenia alebo nedostatočné povolenia.  

Preinštalovanie služby AADConnect pomocou expresných nastavení môže problém rýchlo vyriešiť:

1. [Stiahnite si najnovšiu verziu aplikácie AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Postupujte podľa pokynov pre expresnú inštaláciu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Ďalšie informácie o kontách služby AADConnect nájdete v téme [Azure AD Connect: kontá a povolenia.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
