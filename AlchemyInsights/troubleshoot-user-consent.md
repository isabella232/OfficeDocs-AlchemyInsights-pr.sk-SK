---
title: Riešenie problémov s povolením používateľa
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901630"
---
# <a name="troubleshoot-user-consent"></a>Riešenie problémov s povolením používateľa

1. Môžete nakonfigurovať spôsob, akým koncoví používatelia súhlasia s aplikáciami prostredníctvom platformy Azure Portal alebo PowerShell. Ďalšie informácie nájdete v téme [nastavenia súhlasu používateľa](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Správca môže použiť aj [rozhranie Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) na udelenie súhlasu s delegovanými povoleniami v mene jedného používateľa. Ďalšie informácie nájdete v téme [získanie prístupu v mene používateľa](https://docs.microsoft.com/graph/auth-v2-user).
1. [Chyby týkajúce sa súhlasu používateľa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): v tomto článku sa pojednáva o chybách, ktoré sa môžu vyskytnúť počas procesu odosielania žiadosti. Ak riešite problémy s neočakávaným súhlasom, ktoré neobsahujú žiadne chybové hlásenia, pozrite si tému [scenáre overovania pre Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).