---
title: Vyskytla sa chyba pri overovaní prístupu token chyba počas Desktop Analytics na stravovanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741268"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Došlo k chybe overenie prístupového tokenu" chyba počas Desktop Analytics registrácia

Táto chyba sa zvyčajne pozoruje pri uplynutí tokenu overenia. Zvyčajne obnovuje stránku obnoví token. Tento problém však môže pretrvávať, ak existujú nejaké politiky podmieneného prístupu použité na konto sa používa na palube Desktop Analytics. Môžete skontrolovať Azure AD prihlásiť denníky na portáli Azure zistiť, či existujú nejaké zlyhanie prihlásenia pre konto sa používa pre Desktop Analytics Onboarding.

Ďalšie informácie o podmienenom prístupe nájdete [v téme Plánovanie nasadenia podmieneného prístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).