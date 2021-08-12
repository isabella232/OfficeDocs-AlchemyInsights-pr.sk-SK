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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932112"
---
# <a name="api-permissions-and-consent"></a>Povolenia a súhlas rozhrania API

Aplikácie, ktoré sa integrujú Microsoft identity platform majú oprávnenie na model oprávnenia, ktorý poskytuje používateľom a správcom kontrolu nad spôsobom prístupu k údajom. Implementácia modelu oprávnení sa aktualizovala na webovom Microsoft identity platform koncový bod. Mení, ako musí aplikácia pracovať s Microsoft identity platform. [Povolenia a súhlas v koncovom Microsoft identity platform sa](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) vzťahujú na základné koncepcie tohto modelu oprávnení vrátane rozsahov, povolení a súhlasu.

Rámec [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) zjednodušuje vývoj webových a natívnych klientskych aplikácií s viacerými nájomníkmi. Tieto aplikácie umožňujú prihlásenie pomocou používateľských kont z nájomníka služby Azure AD, ktorý je iný ako ten, v ktorom je aplikácia zaregistrovaná. Okrem vašich vlastných webových rozhraní API budú pravdepodobne potrebovať aj prístup k webovým rozhraniam API spoločnosti Microsoft Graph (na prístup k službe Azure AD, Intune a službám v službách Microsoft 365) a rozhraniam API iných služieb služby Microsoft.

