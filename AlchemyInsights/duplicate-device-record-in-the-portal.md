---
title: Duplicitný záznam zariadenia na portáli
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790172"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplicitný záznam zariadenia na portáli

V prípade, že zariadenie lokalite Správcu konfigurácie správne nenahlási stav spoločnej správy, na portáli sa môžu pre zariadenie zobraziť 2 záznamy. Ak chcete skontrolovať stav spoločnej správy, skontrolujte stĺpec **Spoločná správa** zariadenia v konzole Správcu konfigurácie. Ak sa stĺpec nezobrazuje, môžete ho pridať kliknutím pravým tlačidlom myši na ľubovoľnú hlavičku stĺpca a jeho výberom zo zoznamu.

Hodnota Spoločná správa musí byť **Áno**. Ak je hodnota **Nie**, v klientskom zariadení otvorte aplet klienta Správca konfigurácie a na karte Všeobecné začiarknite políčko **Spoločná správa**.

- Ak je hodnota **Povolené**, označuje to problémy s komunikáciou klienta s bodom správy. Skontrolujte súbor **CcmMessaging.log** v zariadení a preskúmajte možné problémy s pripojením.

- Ak je hodnota **Vypnuté** a zariadenie je zapísané v službe Intune, uistite sa, že zariadenie prijalo politiku spoločnej správy kontrolou súboru **CoManagementHandler.log** v zariadení.
