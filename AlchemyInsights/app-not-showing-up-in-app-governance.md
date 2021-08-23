---
title: Aplikácia sa nezobrazuje v správe aplikácií
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454991"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Aplikácia sa nezobrazuje v správe aplikácií

Ak sa aplikácia nezobrazuje v časti Riadenie aplikácií, skontrolujte toto:

1. Prejdite do [služby Azure AD](https://aad.portal.azure.com/) a vyhľadajte ID aplikácie pre aplikáciu pomocou vyhľadávania názvu aplikácie v hornom paneli na stránke Prehľad.

1. Access Graph Prieskumníka a vyhľadajte ID aplikácie v rámci hlavného id služby pomocou tohto dotazu a nahradením identifikáciou príslušnej <appId> aplikácie: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Ak sa nevrátia žiadne výsledky, pomocou tohto dotazu a nahradením identifikácie príslušnej aplikácie vyhľadajte ID aplikácie v rámci <appId> aplikácie: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Ak sa vyskytnú problémy s dotazom, pozrite si [časť Získanie podpory.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Ďalšie informácie alebo prehľad o aplikáciách v rámci riadenia aplikácií nájdete v téme [Informácie o viditeľnosti a prehľadoch.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Ďalšie informácie o zobrazení aplikácií nájdete v [téme Zobrazenie aplikácií.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
