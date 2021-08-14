---
title: Duplicitný záznam zariadenia na portáli
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004169"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplicitný záznam zariadenia na portáli

V prípade, že zariadenie lokalite Správcu konfigurácie správne nenahlási stav spoločnej správy, na portáli sa môžu pre zariadenie zobraziť 2 záznamy. Ak chcete skontrolovať stav spoločnej správy, skontrolujte stĺpec **Spoločná správa** zariadenia v konzole Správcu konfigurácie. Ak sa stĺpec nezobrazuje, môžete ho pridať kliknutím pravým tlačidlom myši na ľubovoľnú hlavičku stĺpca a jeho výberom zo zoznamu.

Hodnota Spoločná správa musí byť **Áno**. Ak je hodnota **Nie**, v klientskom zariadení otvorte aplet klienta Správca konfigurácie a na karte Všeobecné začiarknite políčko **Spoločná správa**.

- Ak je hodnota **Povolené**, označuje to problémy s komunikáciou klienta s bodom správy. Skontrolujte súbor **CcmMessaging.log** v zariadení a preskúmajte možné problémy s pripojením.

- Ak je hodnota **Vypnuté** a zariadenie je zapísané v službe Intune, uistite sa, že zariadenie prijalo politiku spoločnej správy kontrolou súboru **CoManagementHandler.log** v zariadení.
