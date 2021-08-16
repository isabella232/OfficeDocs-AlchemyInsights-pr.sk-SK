---
title: Nasadenie GPO
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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067855"
---
# <a name="gpo-deployment"></a>Nasadenie GPO

Nastavenia objekty používateľov a počítačov v doménových službách Azure Active Directory (Azure AD DS) sa často spravujú pomocou objektov skupinovej politiky (GPOS). Azure AD DS obsahuje vstavané procesory GPO pre používateľov AADDC a počítače AADDC. Tieto vstavané procesory GPO môžete prispôsobiť tak, aby konfigurovali skupinovú politiku podľa potreby pre vaše prostredie. Členovia skupiny správcov Azure AD DC majú v doméne Azure AD DS oprávnenia na správu skupinovej politiky a môžu tiež vytvárať vlastné procesory GPOS a organizačné jednotky. Ďalšie informácie o tom, čo je skupinová politika a ako funguje, nájdete v téme [Prehľad skupinovej politiky.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

V hybridnom prostredí sa skupinové politiky nakonfigurované v lokálnom prostredí AD DS nesynchronizujú so službou Azure AD DS. Ak chcete definovať nastavenia konfigurácie pre používateľov alebo počítače v Azure AD DS, upravte jeden z predvolených procesorov GPOS alebo vytvorte vlastný objekt GPO.

V tomto článku spravovanie [skupinovej](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) politiky sa uvádza, ako nainštalovať nástroje na správu skupinovej politiky, ako upraviť vstavané procesory GPOS a ako vytvoriť vlastné procesory GPOS.
