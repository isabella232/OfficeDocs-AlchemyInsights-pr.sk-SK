---
title: Prekročený denný limit e-mail. Pracovný postup pozastaví.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514485"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Denné e-mail Limit prekročený. Pracovný postup pozastaví.

Táto chyba môže prijatá v nasledovných prípadoch:

- Máte pracovného postupu SharePoint Online, používajúce SharePoint 2010 alebo SharePoint 2013 pracovného postupu typ platformy.
- Pracovný postup je nakonfigurovaný na odosielanie vlastné e-mailové správy vyše 200 používateľov, viac ako 10 000 príjemcov za deň, alebo viac ako 30 správ za minútu.
- Pri spustení toku činností, e-mailovú správu nie je odoslaná a môžete pozorovať nasledujúce správanie:
    - Pracovného postupu pomocou typ platformy SharePoint 2013, môžete prehľadávať na stránke **Stav toku činností** . Na stránke stav toku činností **Vnútorný stav** je nastavený na **začal**a informácie balón zobrazuje **sa nedá Odoslať príjemcovi**.

Ak chcete obísť tento problém, nakonfigurovať vaše workflow posielať e-maily bez prekročenia [Exchange Online odosielateľa limity](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Napríklad pomocou pauza pracovného postupu, Odoslať e-mail do skupiny Office 365, distribučnú skupinu alebo skupiny zabezpečenia mail zapnuté alebo neodoslať menej než 200 príjemcom naraz.


Ďalšie informácie nájdete v nasledujúcom [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Súvisiace témy
- [Vytvoriť tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 