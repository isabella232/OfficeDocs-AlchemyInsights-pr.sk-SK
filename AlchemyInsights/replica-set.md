---
title: Množina replík
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714590"
---
# <a name="replica-set"></a>Množina replík

AADDS sa nazýva aj spravovaná doména. Je to vlastne dva radiče domén, ktoré sú spustené a udržiavané backendom. Dva radiče domén zahŕňajú jednu hlavnú DC a jednu replikáciu DC. Zálohy v AADDS (spravovaná doména) sú automatizovaný proces spravovaný platformou Azure. V prípade problému s spravovanou doménou vám môže podpora Azure pomôcť pri obnove zo zálohy.

Vytvoríte každú skupinu replík vo virtuálnej sieti. Každá virtuálna sieť musí byť prispôsobená každej inej virtuálnej sieti, ktorá je hostiteľom množiny replík spravovanej domény. V tejto konfigurácii sa vytvorí Topológia siete Mesh, ktorá podporuje replikáciu adresárov. Virtuálna sieť môže podporovať viacero množín replík za predpokladu, že každá množina replík je v inej virtuálnej podsieti.

Ďalšie podrobnosti o skupine replík nájdete v téme [množiny replík konceptov](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
