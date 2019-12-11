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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959509"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Program Outlook sa nemôže pripojiť k verejným priečinkom

Ak prístup k verejnému priečinku nefunguje pre niekoľko používateľov, vyskúšajte nasledujúce kroky:

Pripojiť k EXO PowerShell a nakonfigurovať DefaultPublicFolderMailbox na problémové používateľské konto, aby zodpovedali jeden na pracovné používateľské konto.

Príklad:

Get-poštová schránka WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Súbor schránky ProblemUser-DefaultPublicFolderMailbox \<hodnota z predchádzajúceho príkazu>

Počkajte aspoň jednu hodinu, kým sa zmena prejaví.