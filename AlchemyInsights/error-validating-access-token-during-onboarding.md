---
title: Počas nastupovania do funkcie Desktop Analytics sa vyskytla chyba s overujúca chyba prístupového tokenu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946630"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Počas za panelovania funkcie Desktop Analytics sa vyskytla chyba overovania prístupového tokenu

Táto chyba sa zvyčajne vyskytuje po uplynutí platnosti tokenu overenia. Obnovením stránky sa zvyčajne obnoví token. Tento problém však môže pretrvávať, ak sa v konte používanom na počítačovú analýzu na palube používajú nejaké politiky podmieneného prístupu. Môžete si pozrieť denníky prihlásenia do služby Azure AD na portáli Azure a zistiť, či sa pre konto používaná pre onboardovanie funkcie Desktop Analytics nejaké zlyhanie prihlásenia.

Ďalšie informácie o podmienenom prístupe nájdete v článku [Plánovanie nasadenia podmieneného prístupu.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)