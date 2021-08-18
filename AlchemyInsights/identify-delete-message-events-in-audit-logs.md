---
title: Identifikácia udalostí odstránenia správ v denníkoch auditu
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
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317609"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Denníky auditu pre odstránené e-mailové správy

Od januára 2019 spoločnosť Microsoft predvolene zapína zapisovanie auditu poštovej schránky do denníka. V opačnom prípade ak chcete skontrolovať udalosti odstránenia správ pre konkrétneho používateľa, musíte manuálne povoliť akcie odstránenia pre auditovanie. Ak je zapisovanie auditu poštovej schránky do denníka už vo vašej organizácii alebo pre konkrétneho používateľa povolené, postupujte podľa nasledujúcich krokov.

1. Prihláste sa do [Centra Microsoft 365 súladu](https://protection.office.com/)

2. Kliknite **na položku Vyhľadávanie a skúmanie** a vyberte položku Vyhľadávanie denníka **auditu.**

3. Vyberte rozsah dátumov v **poliach Počiatočný dátum** **a Dátum ukončenia.** Zadajte meno používateľa, ktorého chcete preskúmať (používateľ, ktorý položky odstránil). V poli **Aktivity vyberte** položku Odstránené správy z priečinka Odstránené položky **a Premiestnené** **správy do priečinka Odstránené položky**.

4. Kliknite na **tlačidlo Hľadať**.

Vo výsledkoch vyberte záznam auditu. V letáku s podrobnosťami kliknite na položku **Ďalšie informácie**. Ďalšie informácie o odstránenej položke (napríklad riadok predmetu a umiestnenie položky v prípade jej odstránení) sa zobrazia v poli **Ovplyvnené položky.** Vlastnosť **ClientInfoString** sa zobrazí, ak sa odstránenie vyskytlo v Outlook, Outlook na webe (predtým známe ako Outlook Web App) alebo akomkoľvek inom zariadení.

Ďalšie informácie nájdete v téme Určenie [osoby, ktorá nastavila preposielanie e-mailov v poštovej schránke.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Poznámka:** Odstránené položky nemožno načítať pomocou funkcie denníka auditu. Ak chcete v Outlooku obnoviť odstránené Outlook na webe, pozrite si [časť Obnovenie odstránených položiek v Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
