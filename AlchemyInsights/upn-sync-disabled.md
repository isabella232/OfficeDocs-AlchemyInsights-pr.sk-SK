---
title: Synchronizácia u klienta UPN vypnutá
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038127"
---
# <a name="upn-sync-disabled"></a>Synchronizácia u klienta UPN vypnutá

Ak ste pred 30. marca 2016 začali synchronizáciu so službou Azure AD, spustite túto rutinu typu cmdlet prostredia Azure AD PowerShell, ktorá umožní vašej organizácii softvérové zhody s upnomnom prostredí:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Pre organizácie, ktoré začali synchronizáciu so službou Azure AD 30. marca 2016 alebo po nej, sa automaticky zapne softvérová zhoda s upnovým nastavením.
  
Ďalšie informácie o povolení jemných zhodných nastavení u synchronizačného klienta a ďalších funkciách synchronizácie nájdete v téme [Funkcie služby synchronizácie Azure AD Pripojenie AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

