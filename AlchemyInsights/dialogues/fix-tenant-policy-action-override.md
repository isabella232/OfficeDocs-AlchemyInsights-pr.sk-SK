---
title: Oprava politiky nájomníka (prepísanie akcie)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695694"
---
# <a name="fix-tenant-policy-action-override"></a>Oprava politiky nájomníka (prepísanie akcie)

Táto správa ovplyvnila politiku ochrany pred nevyžiadanou poštou v nájomníkovi. Ak chcete skontrolovať politiku, postupujte takto:

1. Prejdite na [centrum dodržiavania súladu pre Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143)a potom **prejdite do časti**  >    >  [Ochrana pred nevyžiadanou poštou](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Ak chcete zistiť, či **zdroj politiky** označuje nasledovné:  **Pridať-XHeader/ModifySubject/redirect/Delete/žiadna akcia/skrytá správa**

    Ak áno, na karte **vlastné** skontrolujte nastavenie politiky, ktorá ovplyvnila správu. Je možné, že **štandardné nastavenia** aplikované na všetkých zákazníkov služby Exchange Online Protection ovplyvnili správu.

Ďalšie informácie o konfigurácii politiky filtrovania nevyžiadanej pošty nájdete v téme [Konfigurácia politiky filtrovania nevyžiadanej pošty](https://go.microsoft.com/fwlink/?linkid=2101431).
