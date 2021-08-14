---
title: Vlastník nemôže vytvoriť pod priečinok pomocou Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063139"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlastník nemôže vytvoriť pod priečinok pomocou Outlook

**Priebežne sa vyskytuje problém, ktorý sa vyskytuje pri vytváraní podpriečinkov vlastníkmi verejných Outlook. Problém sa čoskoro opraví.**

Zatiaľ použite niektoré z nasledujúcich alternatívnych riešení:

1. Pomocou Outlook pre MAC vytvorte podpriečinok, pretože problém sa bude Outlook iba v prípade počítačových okien (všetky verzie)
2. Správca môže vytvoriť podpriečinok pomocou prostredia EXO Shell alebo EAC
3. Zmena priečinka DefaultPublicFolderMailbox/EffectivePublicFolderMailbox používateľa na inú poštovú schránku ako poštovú schránku obsahu, ktorá spôsobuje problém  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Počkajte jednu hodinu a reštartujte klienta Outlooku