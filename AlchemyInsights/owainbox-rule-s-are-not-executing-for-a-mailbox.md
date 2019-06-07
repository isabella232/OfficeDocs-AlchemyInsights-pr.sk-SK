---
title: 1332 OWA - doručenej pošty pravidiel sa nevykonáva pre poštovú schránku
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762238"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravidlo pre doručenú poštu nefunguje podľa očakávania

Skontrolujte nasledujúce nastavenia:

- Môžu byť presmerované správy poslanej ďalej alebo v odpovediach na automaticky na základe pravidiel pre doručenú poštu iba raz. Presmerovanie pravidlo (pravidlo priečinka doručenej pošty alebo pošty tok pravidlo, tiež známy ako pravidlo prenosu) môžete pridať maximálne desať presmerovanie príjemcov správy. Ďalšie informácie, Zobraziť [Denník, dopravy, a Doručená pošta pravidlo obmedzuje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravidlá pre doručenú poštu nefungujú na alternatívne journaling schránku. Ďalšie informácie o alternatívny journaling schránky, pozri [alternatívne journaling schránku](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Ak chcete vyriešiť tieto problémy, pozri [KB 2829319](https://support.microsoft.com/kb/2829319).

Ak predchádzajúcich vydaniach neuplatníte, spustiť diagnostická zostava pravidlo priečinka doručenej pošty, pred eskalovat vydanie Microsoft Support:

1. Otvorte poštovú schránku v Outlooku na webe, a kliknite na položku **Nastavenie** \> **Možnosti** \> **Usporiadať e-mail** \> **pravidlá pre doručenú poštu**.

2. V spodnej časti stránky, kliknite na tlačidlo **Ak vaše pravidlá nefungujú kliknite tu pre generovanie diagnostickej zostavy**.
