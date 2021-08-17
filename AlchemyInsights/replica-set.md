---
title: Replika množiny
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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110695"
---
# <a name="replica-set"></a>Replika množiny

AADDS sa nazýva aj spravovaná doména. Ide o dva radiče domén, ktoré sú spúšťané a udržiavané backendom. Tieto dva DCs obsahujú jeden hlavný dc a jeden replikáciu DC. Zálohy v službe AADDS (spravovaná doména) je automatizovaný proces spravovaný platformou Azure. V prípade problému so spravovanú doménou vám podpora pre Azure môže pomôcť pri obnovovaní zo zálohy.

Každú množinu repliky vytvoríte vo virtuálnej sieti. Každá virtuálna sieť musí byť peered s každou virtuálnou sieťou, ktorá hosťuje množinu repliky spravovanej domény. Táto konfigurácia vytvorí topológiu siete sieťovej siete, ktorá podporuje replikáciu adresárov. Virtuálna sieť môže podporovať viacero množín replik za predpokladu, že každá množina repliky je v inej virtuálnej podsieti.

Ďalšie informácie o množine repliky nájdete v téme [Množiny repliky konceptov.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
