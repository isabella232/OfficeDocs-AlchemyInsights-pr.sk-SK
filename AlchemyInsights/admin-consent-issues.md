---
title: Problémy s udelením súhlasu správcu
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901511"
---
# <a name="admin-consent-issues"></a>Problémy s udelením súhlasu správcu

1. Povoľte [pracovný postup súhlasu správcu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , aby používatelia mohli požiadať o schválenie správcu priamo z obrazovky súhlasu.

1. Ak sa počas procesu udelenia súhlasu zobrazili neočakávané chyby, v tomto článku nájdete postup na riešenie problémov: [neočakávaná chyba pri vykonávaní súhlasu s aplikáciou](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Ďalšie informácie o [súhlase správcu na platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), o tom, ako funguje [výzva na udelenie súhlasu](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) , a ako [vyhodnotiť žiadosť o súhlas správcu pre celú nájomníka](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Aplikácie, ktoré sú integrované s platformou Microsoft identity, sledujú autorizačný model, ktorý umožňuje používateľom a správcom kontrolovať spôsob prístupu k údajom. Implementácia modelu autorizácie bola aktualizovaná na koncovom bode Microsoft Identity Platform a mení sa, ako musí aplikácia pracovať s platformou Microsoft Identity. Pozrite si tému [povolenia a súhlas v koncovom bode platformy Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) pre prehľad tohto modelu autorizácie vrátane rozsahov, povolení a súhlasu.