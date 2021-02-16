---
title: Skupinová politika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256905"
---
# <a name="group-policy"></a>Skupinová politika

Nastavenia pre objekty používateľov a počítača v doménových službách Azure Active Directory (Azure AD DS) sa často spravujú pomocou objektov skupinovej politiky (GPO). Azure AD DS obsahuje vstavané objekty GPO pre AADDC používateľov a kontajnery na AADDC počítače. Tieto vstavané GPOs môžete prispôsobiť tak, aby sa Skupinová politika podľa potreby nakonfigurovala pre vaše prostredie. Členovia skupiny Správcovia služby Azure AD DC majú oprávnenia na správu skupinovej politiky v doméne Azure AD DS a môžu tiež vytvárať vlastné GPOs a organizačné jednotky (organizačné jednotky). Ďalšie informácie o tom, čo je Skupinová politika a ako funguje, nájdete v téme [Prehľad skupinovej politiky](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

V hybridnom prostredí sa skupinové politiky nakonfigurované v lokálnom prostredí AD DS nesynchronizujú so službou Azure AD DS. Ak chcete definovať nastavenia konfigurácie pre používateľov alebo počítače v službe Azure AD DS, upravte niektorú z predvolených GPOs alebo vytvorte vlastný objekt GPO.

V tomto článku sa [spravuje Skupinová politika](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) , ktorá vám ukáže, ako nainštalovať nástroje na správu skupinovej politiky, ako Tony upraviť vstavané GPOs a ako vytvoriť vlastné GPOs.



