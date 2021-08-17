---
title: 932 Inovácia AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104827"
---
# <a name="upgrade-azure-ad-connect"></a>Inovácia služby Azure AD Pripojenie

Automatická inovácia je predvolene povolená pre Azure AD Pripojenie, čo pomáha zabezpečiť, že používate najnovšiu verziu. Ak chcete overiť nastavenia automatickej inovácie, použite rutinu typu cmdlet **Get-ADSyncAutoUpgrade** v prostredí Azure AD PowerShell. Rutina typu cmdlet vráti jednu z nasledujúcich hodnôt:

- **Povolené:** Automatická inovácia je povolená.

- **Vypnuté:** Automatická inovácia je vypnutá.

- **Pozastavené:** Systém už nie je oprávnený na prijímanie automatických aktualizácií. Túto hodnotu nie je možné nakonfigurovať. je nastavený systémom.

Ďalšie informácie nájdete v téme [Automatická inovácia.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Ak si chcete stiahnuť najnovšiu verziu služby Azure AD Pripojenie, prejdite [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) na .
