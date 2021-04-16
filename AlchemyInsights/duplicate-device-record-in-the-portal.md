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
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814531"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplicitný záznam zariadenia na portáli

V prípade, že zariadenie lokalite Správcu konfigurácie správne nenahlási stav spoločnej správy, na portáli sa môžu pre zariadenie zobraziť 2 záznamy. Ak chcete skontrolovať stav spoločnej správy, skontrolujte stĺpec **Spoločná správa** zariadenia v konzole Správcu konfigurácie. Ak sa stĺpec nezobrazuje, môžete ho pridať kliknutím pravým tlačidlom myši na ľubovoľnú hlavičku stĺpca a jeho výberom zo zoznamu.

Hodnota Spoločná správa musí byť **Áno**. Ak je hodnota **Nie**, v klientskom zariadení otvorte aplet klienta Správca konfigurácie a na karte Všeobecné začiarknite políčko **Spoločná správa**.

- Ak je hodnota **Povolené**, označuje to problémy s komunikáciou klienta s bodom správy. Skontrolujte súbor **CcmMessaging.log** v zariadení a preskúmajte možné problémy s pripojením.

- Ak je hodnota **Vypnuté** a zariadenie je zapísané v službe Intune, uistite sa, že zariadenie prijalo politiku spoločnej správy kontrolou súboru **CoManagementHandler.log** v zariadení.
