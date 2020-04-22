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
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716511"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Denníky auditu pre odstránené e-mailové správy

Od januára 2019, Microsoft je Zapnutie poštovej schránky auditu zapisovania do denníka v predvolenom nastavení. V opačnom prípade môžete skontrolovať odstránenie udalostí správy pre konkrétneho používateľa, musíte manuálne povoliť akcie odstránenia pre auditovanie. Ak poštovej schránky auditu zapisovania je už povolená pre vašu organizáciu alebo pre konkrétneho používateľa, postupujte podľa nasledujúcich krokov.

1. Prihláste sa do [Microsoft 365 zabezpečenia & Compliance Center](https://protection.office.com/)

2. Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte položku **vyhľadávanie denníkov auditu**.

3. Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Dátum ukončenia** . Zadajte používateľské meno používateľa, ktorý chcete zistiť (používateľ, ktorý odstránil položky). V poli **aktivity** vyberte položku **odstránené správy z priečinka Odstránené položky** a **premiestnili sa správy do priečinka Odstránené položky**.

4. Kliknite na tlačidlo **Hľadať**.

Vo výsledkoch vyberte záznam auditu. V rozbaľovacom zozname Podrobnosti kliknite na položku **Ďalšie informácie**. Ďalšie informácie o odstránenej položke (napríklad riadok predmetu a umiestnenie položky pri jej odstránení) sa zobrazia v poli **Affecteditems** . Vlastnosť **Clientinfostring** sa zobrazí, ak sa odstránenie vyskytlo v programe Outlook, Outlook na webe (predtým označované ako aplikácia Outlook Web App) alebo v akomkoľvek inom zariadení.

Ďalšie informácie nájdete v téme [určenie, kto nastaviť presmerovanie e-mailov pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Poznámka**: odstránené položky nie je možné načítať pomocou funkcie denník auditu. Ak chcete obnoviť odstránené správy v programe Outlook na webe, pozrite si ďalšie informácie [v téme Obnovenie odstránených položiek v aplikácii Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
