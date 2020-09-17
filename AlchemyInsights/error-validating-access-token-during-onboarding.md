---
title: Pri overovaní chyby tokenu prístupu počas analýzy počítača sa vyskytla chyba.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783566"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Chyba pri overovaní accessového tokenu sa vyskytla chyba počas integrovaného nástroja na analýzu pracovnej plochy

Táto chyba sa zvyčajne sleduje po uplynutí platnosti overovacieho tokenu. Obnovenie stránky zvyčajne obnoví token. Tento problém však môže pretrvávať, ak sa uplatňujú politiky podmieneného prístupu použité na konto, ktoré sa používa na analýzu na palube počítača. Ak chcete zistiť, či existujú nejaké zlyhanie prihlásenia pre konto, ktoré sa používa na zabudovanie počítačovej analýzy, môžete si pozrieť Denníky prihlásenia Azure AD na portáli Azure Portal.

Ďalšie informácie o podmienenom prístupe nájdete v téme [Plánovanie nasadenia podmieneného prístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).