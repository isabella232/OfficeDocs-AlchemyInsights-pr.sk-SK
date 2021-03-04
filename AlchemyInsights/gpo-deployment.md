---
title: Nasadenie objektu GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428053"
---
# <a name="gpo-deployment"></a>Nasadenie objektu GPO

Nastavenia pre objekty používateľov a počítača v doménových službách Azure Active Directory (Azure AD DS) sa často spravujú pomocou objektov skupinovej politiky (GPO). Azure AD DS obsahuje vstavané objekty GPO pre AADDC používateľov a kontajnery na AADDC počítače. Tieto vstavané GPOs môžete prispôsobiť tak, aby sa Skupinová politika podľa potreby nakonfigurovala pre vaše prostredie. Členovia skupiny Správcovia služby Azure AD DC majú oprávnenia na správu skupinovej politiky v doméne Azure AD DS a môžu tiež vytvárať vlastné GPOs a organizačné jednotky (organizačné jednotky). Ďalšie informácie o tom, čo je Skupinová politika a ako funguje, nájdete v téme [Prehľad skupinovej politiky](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

V hybridnom prostredí sa skupinové politiky nakonfigurované v lokálnom prostredí AD DS nesynchronizujú so službou Azure AD DS. Ak chcete definovať nastavenia konfigurácie pre používateľov alebo počítače v službe Azure AD DS, upravte niektorú z predvolených GPOs alebo vytvorte vlastný objekt GPO.

V tomto článku sa [spravuje Skupinová politika](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) , ktorá vám ukáže, ako nainštalovať nástroje na správu skupinovej politiky, ako Tony upraviť vstavané GPOs a ako vytvoriť vlastné GPOs.
