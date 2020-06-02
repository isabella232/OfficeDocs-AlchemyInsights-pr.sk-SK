---
title: Identifikácia udalostí odstránenia správy v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509003"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Denníky auditu odstránených e-mailových správ

Od januára 2019, Microsoft predvolene zapína zapisovanie do denníka auditu poštovej schránky. Ak chcete skontrolovať udalosti správy pre konkrétneho používateľa, musíte manuálne povoliť akcie odstránenia na auditovanie. Ak poštovej schránky auditu zapisovania do denníka je už povolená pre vašu organizáciu alebo pre konkrétneho používateľa, postupujte podľa krokov uvedených nižšie.

1. Prihláste sa do [Centra súladu zabezpečenia & microsoft 365](https://protection.office.com/)

2. Kliknite na **položku Vyhľadávanie a vyšetrovanie** a vyberte položku **Hľadať denník auditu**.

3. Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum.** Zadajte meno používateľa, ktorého chcete preskúmať (používateľa, ktorý položky odstránil). V poli **Aktivity** vyberte položku **Odstránené správy z priečinka Odstránené položky** a **Premiestniť správy do priečinka Odstránené položky**.

4. Kliknite na tlačidlo **Hľadať**.

Vo výsledkoch vyberte záznam auditu. V rozbaľovacom zozname podrobností kliknite na položku **Ďalšie informácie**. Ďalšie informácie o odstránenej položke (napríklad predmet a umiestnenie položky pri jej odstránení) sa zobrazia v poli **AffectedItems.** Vlastnosť **ClientInfoString** sa zobrazí, ak sa odstránenie vyskytlo v programe Outlook, Outlook na webe (predtým známa ako aplikácia Outlook Web App) alebo v akomkoľvek inom zariadení.

Ďalšie informácie sa nachádzajú v téme [Určenie osôb, ktoré nastavia preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Poznámka:** Odstránené položky nie je možné načítať pomocou funkcie denníka auditu. Informácie o načítanie odstránených správ v Outlooku na webe nájdete v téme [Obnovenie odstránených položiek v aplikácii Aplikácia Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
