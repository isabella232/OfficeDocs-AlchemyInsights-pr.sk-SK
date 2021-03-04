---
title: Vyhľadanie udalostí vykonaných na základe pravidiel pre doručenú poštu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430016"
---
# <a name="find-events-performed-on-inbox-rules"></a>Vyhľadanie udalostí vykonaných na základe pravidiel pre doručenú poštu

Keď sa pravidlá pre doručenú poštu vytvoria, zmenia alebo odstránia, udalosti sa zaznamenávajú do denníka auditu. Tu je návod na ich preskúmanie:

1. Prejdite na [centrum dodržiavania súladu & zabezpečenia služieb Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Vyberte položku Hľadať > denník auditu.

    > [!NOTE]
    > Ak sa zobrazí oznámenie o tom, že je potrebné zapnúť auditovanie, pokračujte a teraz ho zapnite. Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť vytiahnuť údaje z predchádzajúcich dátumov.
1. Vyberte pole aktivity a vyhľadajte položku aktivity poštovej schránky servera Exchange a potom vyberte položku New-InboxRule vytvoriť pravidlo pre doručenú poštu z aplikácie Outlook Web App. Po dokončení kliknite mimo tably na minimalizovanie tably aktivity.
1. Zadajte rozsah dátumov a potom v poli používatelia vyberte meno používateľa, ktorého chcete preskúmať. Naraz môžete vybrať viac ako jedného používateľa.
1. Vyberte položku Hľadať. Aktivity sa zobrazia v časti výsledky.
1. Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku Ďalšie informácie. V časti parametre sa zobrazuje názov pravidla, podmienky a akcie, ktoré bude mať pravidlo.

Ďalšie informácie nájdete v téme Vyhľadávanie v denníku auditu služieb Office 365 na riešenie bežných scenárov.