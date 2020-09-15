---
title: Identifikácia odstraňovania udalostí správy v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696528"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Denníky auditu odstránených e-mailových správ

Od januára 2019 spoločnosť Microsoft zapne zapisovanie do denníka auditu poštovej schránky na základe predvoleného nastavenia. Ak v opačnom prípade chcete skontrolovať odstránenie udalostí správy pre konkrétneho používateľa, musíte manuálne povoliť akcie odstránenia na auditovanie. Ak je zapisovanie do denníka auditu poštovej schránky pre vašu organizáciu alebo konkrétneho používateľa už zapnuté, postupujte podľa nižšie uvedených krokov.

1. Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/)

2. Kliknite na položku **vyhľadávanie a šetrenie** a vyberte položku **vyhľadávanie denníkov auditu**.

3. V poliach **Počiatočný** dátum a **Koncový dátum** vyberte rozsah dátumov. Zadajte meno používateľa, ktoré chcete preskúmať (používateľ, ktorý odstránil položky). V poli **aktivity** vyberte položku **odstránené správy z priečinka Odstránené položky** a **premiestnené správy do priečinka Odstránené položky**.

4. Kliknite na položku **Hľadať**.

Vo výsledkoch vyberte záznam auditu. V rozbaľovacom zozname Podrobnosti kliknite na položku **Ďalšie informácie**. Ďalšie informácie o odstránenej položke (napríklad riadok predmetu a umiestnenie položky pri odstránení) sa zobrazia v poli **AffectedItems** . Vlastnosť **ClientInfoString** sa zobrazí, ak sa v Outlooku, Outlooku na webe (predtým známy ako Outlook Web App) alebo v ľubovoľnom inom zariadení zobrazuje odstránenie.

Ďalšie informácie nájdete v téme [Určenie používateľov, ktorí nastavujú preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Poznámka**: odstránené položky nie je možné načítať pomocou funkcie denník auditu. Ak chcete obnoviť odstránené správy v Outlooku na webe, prečítajte si tému [Obnovenie odstránených položiek v aplikácii Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
