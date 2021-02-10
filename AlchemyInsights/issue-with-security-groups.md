---
title: Problém so skupinami zabezpečenia
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177632"
---
# <a name="issue-with-security-groups"></a>Problém so skupinami zabezpečenia

**Ak dostávate AADDS104 chyby siete**

Neplatné pravidlá skupiny zabezpečenia siete sú najčastejšou príčinou chýb siete pre doménové služby Azure Active Directory (AD DS). Skupina zabezpečenia siete pre virtuálnu sieť musí umožniť prístup k konkrétnym portom a protokolom. Ak sú tieto porty blokované, platforma Azure nedokáže monitorovať alebo aktualizovať spravovanú doménu. Synchronizácia medzi službou Azure AD a službou Azure AD DS je tiež ovplyvnená. Zabezpečte, aby boli predvolené porty otvorené, aby sa zabránilo prerušeniu prevádzky.

Ak chcete porozumieť a vyriešiť bežné upozornenia na problémy s konfiguráciou skupiny zabezpečenia siete, pozrite si tému [Pridanie a overenie skupín zabezpečenia](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
