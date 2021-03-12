---
title: Príklad Microsoft Defendera pre politiku bezpečného pripojenia služieb Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749197"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Príklad Microsoft Defendera pre politiku bezpečného pripojenia služieb Office 365

Tieto nastavenia umožňujú politiku s názvom *žiadne oneskorenia* , ktoré okamžite doručujú správy a potom po ich naskenovaní opätovne priloží prílohy:

- **Názov**: žiadne oneskorenia
- **Popis**: doručí správy okamžite a opätovne priloží prílohy po kontrole.
- **Odpoveď**: vyberte možnosť **dynamické doručenie** . Ďalšie informácie nájdete v téme [dynamické doručenie v zásadách bezpečných príloh](https://go.microsoft.com/fwlink/?linkid=2092328).
- Sekcia **presmerovať prílohu** : vyberte možnosť na **povolenie presmerovania** a potom zadajte e-mailovú adresu globálneho správcu služieb Microsoft 365, správcu zabezpečenia alebo bezpečnostného analytika, ktorý bude skúmať nebezpečné prílohy.
- **Použiť na** sekciu: vyberte **doménu príjemcu** a potom vyberte svoju doménu. Vyberte položku **Pridať** a potom kliknite na **tlačidlo OK**. Po dokončení vyberte položku **Uložiť**.

Ďalšie informácie nájdete v téme [bezpečné prílohy v programe Microsoft Defender pre Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
