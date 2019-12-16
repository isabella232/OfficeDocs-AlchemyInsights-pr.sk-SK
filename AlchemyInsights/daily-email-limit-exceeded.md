---
title: Prekročený denný limit e-mailov. Pracovný postup je pozastavený.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053132"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Prekročený denný limit e-mailov. Pracovný postup je pozastavený.

Táto chyba môže byť prijatá v nasledovných prípadoch:

- Máte pracovný postup SharePoint Online, ktorý používa typ platformy SharePoint 2010 alebo SharePoint 2013 pracovného postupu.
- Pracovný postup je nakonfigurovaný na odoslanie vlastnej e-mailovej správy na viac ako 200 používateľov naraz, viac ako 10 000 príjemcov za deň, alebo viac ako 30 správ za minútu.
- Pri spustení pracovného postupu, e-mailová správa nie je odoslaná a zistíte nasledovné správanie:
    - Pre tok činností pomocou typu platformy SharePoint 2013, môžete prechádzať na stránke **stav pracovného postupu** . Na stránke stav toku činností je **interný stav** nastavený na hodnotu **spustené**a informačný balón sa **nedá Odoslať príjemcovi**.

Tento problém obísť, nakonfigurujte pracovný postup na odosielanie e-mailových správ bez prekročenia [limitov odosielateľa Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Napríklad, použite pauzu v toku činností, pošlite e-mail do skupiny Office 365, distribučnej skupiny alebo poštové skupiny zabezpečenia povolené alebo Odoslať správu menej ako 200 príjemcov naraz.


Ďalšie informácie nájdete v nasledujúcom [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Súvisiace témy
- [Vytvoriť tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 