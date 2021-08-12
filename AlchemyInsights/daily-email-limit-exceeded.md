---
title: Prekročil sa denný limit e-mailov. Pracovný postup je pozastavený.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914666"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Prekročený denný limit e-mailov. Pracovný postup je pozastavený.

Táto chyba sa môže zobraziť v nasledujúcich scenároch:

- V SharePoint Online máte pracovný postup, ktorý používa typ platformy SharePoint 2010 alebo SharePoint 2013.
- Pracovný postup je nakonfigurovaný na odosielanie vlastnej e-mailovej správy viac ako 200 používateľom naraz, viac ako 10 000 príjemcom za deň alebo viac než 30 správ za minútu.
- Keď spustíte pracovný postup, e-mailová správa sa odošle a všimnete si nasledujúce správanie:
    - V prípade pracovného postupu, ktorý používa typ SharePoint 2013, prejdite na stránku **Stavu pracovného** postupu. Na stránke stavu pracovného postupu je  **interný stav** nastavený na položku Spustené a v informačnom bubline sa zobrazí hlásenie Nie je **možné odoslať príjemcovi.**

Ak chcete tento problém obísť, nakonfigurujte pracovný postup na odosielanie e-mailových správ bez toho, aby [Exchange Online limity odosielateľov.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Môžete napríklad použiť prestávku v pracovnom postupe, odoslať e-mail skupine Microsoft 365, distribučnej skupine alebo skupine zabezpečenia s podporou e-mailu alebo odoslať správu menej ako 200 príjemcom súčasne.


Ďalšie informácie nájdete v nasledujúcom [článku.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Súvisiace témy
- [Vytvorenie Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 