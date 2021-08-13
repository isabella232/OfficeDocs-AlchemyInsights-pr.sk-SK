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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937116"
---
# <a name="active-directory-not-syncing"></a>Nesynchronizuje sa Active Directory

Ak sa vám zobrazuje chyba synchronizácie, napríklad "žiadna nedávna synchronizácia" alebo ak si všimnete stav synchronizácie adresárov na portáli pre správcov služieb Office zobrazí hlásenie Posledná synchronizácia pred viac ako 3 dňami, môže to byť preto, že AADConnect má nesprávne nastavenia alebo nedostatočné povolenia na vykonanie synchronizácie.  

Preinštalovanie služby AADConnect pomocou expresných nastavení môže tento problém rýchlo vyriešiť:

1. [Stiahnite si najnovšiu verziu aplikácie AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Postupujte podľa pokynov pre expresnú inštaláciu.](/azure/active-directory/hybrid/how-to-connect-install-express)

Nástroj Azure AD Connect musí byť nainštalovaný v systéme Windows Server 2012 alebo novšom. Tento server musí byť pripojený k doméne a môže to byť radič domény alebo členský server. Úplný zoznam požiadaviek a predpokladov služby Azure AD Pripojenie AD nájdete v článku [Predpoklady pre Azure AD Pripojenie.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Ďalšie informácie o kontách služby AADConnect nájdete v téme [Azure AD Pripojenie: Kontá a povolenia.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
