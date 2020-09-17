---
title: 932 inovácia AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806054"
---
# <a name="upgrade-azure-ad-connect"></a>Inovácia služby Azure AD Connect

Predvolene je povolená Automatická inovácia pre službu Azure AD Connect, ktorá pomáha zabezpečiť, že máte nainštalovanú najnovšiu verziu. Ak chcete overiť nastavenia automatickej inovácie, použite rutinu typu cmdlet **Get-ADSyncAutoUpgrade** v prostredí Azure AD PowerShell. Rutina typu cmdlet vráti jednu z nasledujúcich hodnôt:

- **Povolené**: Automatická inovácia je povolená.

- **Vypnuté**: Automatická inovácia je zakázaná.

- **Pozastavené**: systém už nie je oprávnený prijímať automatické inovácie. Túto hodnotu nie je možné nakonfigurovať. je nastavený systémom.

Ďalšie informácie nájdete v téme [Automatická inovácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Ak si chcete stiahnuť najnovšiu verziu služby Azure AD Connect, prejdite na položku [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
