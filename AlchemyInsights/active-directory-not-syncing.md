---
title: Služba Active Directory sa nesynchronizuje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265271"
---
# <a name="active-directory-not-syncing"></a>Služba Active Directory sa nesynchronizuje

Ak dostávate chyby synchronizácie, napríklad "žiadna Nedávna synchronizácia" alebo oznámenie stav synchronizácie adresárov na portáli Office Admin hovorí: "naposledy synchronizované viac ako 3 dni," môže byť, že AADConnect má nesprávne nastavenia alebo nedostatočné povolenia na vykonanie synchronizácie.  

Preinštalovanie AADConnect pomocou expresné nastavenie môže vyriešiť problém rýchlo:

1. [Prevezmite si najnovšiu verziu AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Postupujte podľa pokynov na expresnú inštaláciu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Ďalšie informácie o kontách služby AADConnect nájdete v téme [Azure AD Connect: kontá a povolenia](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
