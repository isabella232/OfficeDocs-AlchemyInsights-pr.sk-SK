---
title: Riešenie problémov so súhlasom používateľa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007913"
---
# <a name="troubleshoot-user-consent"></a>Riešenie problémov so súhlasom používateľa

1. Prostredníctvom portálu Azure alebo prostredia PowerShell môžete nakonfigurovať súhlas koncových používateľov s aplikáciami. Ďalšie [informácie nájdete v téme](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) Nastavenia súhlasu používateľa.
1. Správca môže tiež použiť [rozhranie MICROSOFT Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) na udelenie súhlasu s delegovanými povoleniami v mene jedného používateľa. Ďalšie informácie nájdete v [téme Získanie prístupu v mene používateľa.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Chyby súhlasu používateľa:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)Tento článok popisuje chyby, ktoré sa môžu vyskytnúť počas procesu súhlasu s aplikáciou. Ak sa pri riešení problémov neočakávané výzvy na súhlas, ktoré neobsahujú žiadne chybové hlásenia, pozrite si [časť Scenáre overovania pre Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)