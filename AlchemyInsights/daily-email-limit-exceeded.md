---
title: Prekročil sa limit denného e-mailu. Pracovný postup sa pozastavuje.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731578"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Prekročil sa limit denného e-mailu. Pracovný postup sa pozastavuje.

Táto chyba môže byť prijatá v nasledovných prípadoch:

- Máte pracovný postup v SharePointe Online, ktorý používa typ platformy pracovného postupu SharePointu 2010 alebo SharePoint 2013.
- Pracovný postup je nakonfigurovaný na odoslanie vlastnej e-mailovej správy viacerým používateľom vo 200, viac ako 10 000 príjemcov za deň alebo viac ako 30 správ za minútu.
- Po spustení pracovného postupu sa e-mailová správa neodošle a všimnete si nasledovné správanie:
    - Ak používate pracovný postup s použitím typu platformy SharePoint 2013, prejdite na stránku **stavu pracovného postupu** . Na stránke stav pracovného postupu je **vnútorný stav** nastavený na možnosť **Spustiť**a v bubline s informáciami sa **nedajú Odoslať príjemcovi**.

Ak chcete tento problém obísť, nakonfigurujte pracovný postup na odosielanie e-mailových správ bez prekročenia [limitov odosielateľov služby Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Môžete napríklad použiť pauzu v pracovnom postupe, Odoslať e-mail do skupiny Microsoft 365, distribučnej skupiny alebo skupiny zabezpečenia s podporou e-mailu alebo Odoslať správu menej ako 200 príjemcom naraz.


Ďalšie informácie nájdete v nasledujúcom [článku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Súvisiace témy
- [Vytvorenie toku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 