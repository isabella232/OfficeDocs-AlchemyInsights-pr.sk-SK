---
title: Denný limit e-mailu bol prekročený. Pracovný postup je pozastavený.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580348"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Denný limit e-mailu prekročený. Pracovný postup je pozastavený.

Táto chyba môže byť prijaté v nasledujúcich situáciách:

- Máte pracovný postup sharepointonline, ktorý používa typ platformy SharePoint 2010 alebo SharePoint 2013 pracovného postupu.
- Pracovný postup je nakonfigurovaný na odosielanie vlastnej e-mailovej správy viac ako 200 používateľom naraz, viac ako 10 000 príjemcov za deň alebo viac ako 30 správ za minútu.
- Keď spustíte pracovný postup, e-mailová správa sa neodošle a zistíte nasledovné správanie:
    - Pracovný postup pomocou typu platformy SharePoint 2013, prejdite na stránku **stav pracovného postupu.** Na stránke Stav pracovného postupu je **interný stav** nastavený na **hodnotu Spustené**a informačný bublina zobrazuje **položku Nedá sa odoslať príjemcovi**.

Tento problém obísť, nakonfigurujte pracovný postup na odosielanie e-mailových správ bez prekročenia [limitov odosielateľa Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Použite napríklad pauzu v pracovnom postupe, odošlite e-mail skupine Microsoft 365, distribučnej skupine alebo skupine zabezpečenia s podporou pošty alebo odošlite správu naraz menej ako 200 príjemcom.


Ďalšie informácie nájdete v nasledujúcom [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Súvisiace témy
- [Vytvoriť tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a postup](https://flow.microsoft.com/blog/sharepoint-and-flow/) 