---
title: Manuálne prihlásenie do prehliadača Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678850"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Manuálne prihlásenie do prehliadača Microsoft Edge

Ak sa používateľ pri prvom spustení neprihlásite automaticky, používateľ sa môže prihlásiť manuálne prostredníctvom nastavení prehliadača alebo cez rozbaľovacie tlačidlo identita. Ak chcete spravovať prihlásenie, použite tieto podmienky:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -Ak chcete, aby mal používateľ vždy pracovný profil v prehliadači Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – obmedzenie prihlásenia do množiny dôveryhodných kont.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -Ak chcete zakázať prihlásenie alebo prinútiť používateľov, aby sa prihlásili.

