---
title: Nie je možné získať prístup k verejným priečinkom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891764"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Program Outlook sa nemôže pripojiť k verejným priečinkom

Ak prístup k verejnému priečinku nefunguje niektorým používateľom, vyskúšajte nasledujúce kroky:

Pripojiť k EXO PowerShell a nakonfigurovať parameter DefaultPublicFolderMailbox na problémové používateľské konto, aby zodpovedali parametra na pracovné používateľské konto.

Príklad:

Get-poštová schránka WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Súbor schránky ProblemUser-DefaultPublicFolderMailbox \<hodnota z predchádzajúceho príkazu>

Počkajte aspoň jednu hodinu, kým sa zmena prejaví.

Ak problém pretrváva, postupujte podľa [tohto postupu](https://aka.ms/pfcte) a Vyriešte problémy s prístupom k verejným priečinkom pomocou programu Outlook.