---
title: V Centre zabezpečenia sa nenašli žiadne správy o predplatných
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544123"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>V Centre zabezpečenia sa nenašli žiadne správy o predplatných

Ak sa počas prístupu k Centrum zabezpečenia v programe Microsoft Defender zobrazí hlásenie Nenašli sa žiadne predplatné, znamená to, že Azure Active Directory (AAD) používaný na prihlásenie používateľa na portál nemá licenciu na Microsoft Defender ATP.  

Licencie Windows E5 a Office E5 sú samostatné licencie.

Otvorte prípad podpory, ak bola licencia zakúpená, ale nie je ustavená v tejto inštancii služby AAD. Či už máte: <br/>
-   Možný problém s poskytovaním licencií.<br/>
-   Neúmyselne ste licenciu zverejňujú inej službe Microsoft AAD ako ten, ktorý sa používa na overovanie do služby.