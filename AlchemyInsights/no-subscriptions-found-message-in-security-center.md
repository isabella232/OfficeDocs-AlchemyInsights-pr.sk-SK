---
title: V centre zabezpečenia nie sú nájdené žiadne predplatné
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713965"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>V centre zabezpečenia nie sú nájdené žiadne predplatné

Ak sa pri prístupe k centru zabezpečenia programu Microsoft Defender zobrazí hlásenie žiadne nájdené predplatné, znamená to, že v službe Azure Active Directory (AAD), ktorá sa používa na prihlásenie používateľa na portál, nie je k dispozícii licencia Microsoft Defender ATP.  

Licencie na Windows E5 a Office E5 sú samostatné licencie.

Otvorte prípad podpory, ak bola licencia zakúpená, ale nebola poskytnutá tejto inštancii AAD. Buď máte: <br/>
-   Možný problém s poskytovaním licencií.<br/>
-   Ste neúmyselne ustanovili licenciu na inú spoločnosť Microsoft AAD, než je tá, ktorá sa použila na overenie do služby.