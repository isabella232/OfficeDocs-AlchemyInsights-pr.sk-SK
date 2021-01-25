---
title: Povolenia a súhlas rozhrania API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974993"
---
# <a name="api-permissions-and-consent"></a>Povolenia a súhlas rozhrania API

Aplikácie, ktoré sú integrované s platformou Microsoft identity, sledujú autorizačný model, ktorý umožňuje používateľom a správcom kontrolovať spôsob prístupu k údajom. Implementácia modelu autorizácie bola aktualizovaná na koncovom bode platformy Microsoft Identity. Zmení sa, ako aplikácia musí pracovať s platformou Microsoft Identity. [Povolenia a súhlas v koncovom bode platformy Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) sa vzťahujú na základné pojmy tohto modelu autorizácie vrátane rozsahov, povolení a súhlasu.

[Rámec súhlasu služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) zjednodušuje tvorbu webových a natívnych klientskych aplikácií viacerých nájomníkov. Tieto aplikácie povoľujú prihlásenie pomocou používateľských kont z nájomníka služby Azure AD, ktorý sa líši od toho, v ktorom je aplikácia zaregistrovaná. Okrem vlastných webových rozhraní API môžu tiež potrebovať prístup k webovým rozhraniam API, ako je napríklad rozhranie Microsoft Graph API (na prístup k službe Azure AD, Intune a službám v Microsoft 365) a v iných rozhraniach API služieb spoločnosti Microsoft.

