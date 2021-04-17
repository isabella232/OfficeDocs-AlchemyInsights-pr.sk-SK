---
title: Vlastník nemôže vytvoriť pod priečinok pomocou programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836150"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlastník nemôže vytvoriť pod priečinok pomocou programu Outlook

**Priebežne sa vyskytuje problém, ktorý sa vyskytuje pri vytváraní podpriečinkov vlastníkmi verejných priečinkov pomocou Outlooku. Problém sa čoskoro opraví.**

Zatiaľ použite niektoré z nasledujúcich alternatívnych riešení:

1. Pomocou Outlooku pre MAC vytvorte podpriečinok, keďže problém ovplyvňuje iba Outlook pre stolné okná (všetky verzie)
2. Správca môže vytvoriť podpriečinok pomocou prostredia EXO Shell alebo EAC
3. Zmena priečinka DefaultPublicFolderMailbox/EffectivePublicFolderMailbox používateľa na inú poštovú schránku ako poštovú schránku obsahu, ktorá spôsobuje problém  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Počkajte jednu hodinu a reštartujte klienta Outlooku