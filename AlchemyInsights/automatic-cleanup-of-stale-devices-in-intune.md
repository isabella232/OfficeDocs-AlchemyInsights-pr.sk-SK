---
title: Automatické čistenie zastaraných zariadení v intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555733"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatické čistenie zastaraných zariadení v intune

Intune umožňuje správcovi nakonfigurovať časový interval medzi 90 a 270 dňami, po ktorom sa zo služby odstránia zastarané zariadenia. Toto nastavenie je organizácia široká a po aktivácii nadobúda účinnosť okamžite. Všetky zariadenia, ktoré nie sú kontrolované na serveri Intune po dobu presahujúcu nastavenie sa natrvalo odstránia.

**Upozornenie:** Iba objekty zariadenia MDM sú vhodné pre túto akciu čistenia. EAS iba objekty zariadenia sú vylúčené.

Ďalšie informácie o tom, kedy sa zariadenie stane spôsobilým na vymazanie na základe nastavenia zariadenia na čistenie a jeho "stavu":

Nastavenie: **Odstrániť zariadenia po dátume poslednej registrácie: Áno (niektoré hodnoty (N) v zadaných dňoch)**

- Na základe hodnoty (N) nakonfigurovanej v nastavení služba Intune odstráni zariadenie v zadaných dňoch po tom, ako sa naposledy úspešne skontroluje.

Nastavenie: **Odstrániť zariadenia po poslednej registrácii dátum: Nie**

- 180 dní po vypršaní platnosti certifikátu zariadenia a neobnoví sa, zariadenie sa odstráni.

**Upozornenie:** V oboch prípadoch musí byť zariadenie úspešne zaregistrované v intune. Registrácia sa vyskytuje počas prvého zariadenia checkin so službou Intune.

Ak sa zariadenie úspešne zaregistruje do intune, ale neregistruje sa intune, zariadenie sa odstráni 270 dní po registrácii. (90 dní na označenie zariadenia ako zrušené a ďalších 180 dní na odstránenie záznamu.)

V konzole Intune momentálne neexistuje mechanizmus na stanovenie dátumu uplynutia platnosti certifikácie zariadenia pre dané zariadenie.