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
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782166"
---
# <a name="upn-sync-disabled"></a>Synchronizácia u klienta UPN vypnutá

Ak ste pred 30. marca 2016 začali synchronizáciu so službou Azure AD, spustite túto rutinu typu cmdlet prostredia Azure AD PowerShell, ktorá umožní vašej organizácii softvérové zhody s upnomnom prostredí:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Pre organizácie, ktoré začali synchronizáciu so službou Azure AD 30. marca 2016 alebo po nej, sa automaticky zapne softvérová zhoda s upnovým nastavením.
  
Ďalšie informácie o povolení jemných zhodných nastavení u synchronizačného klienta a ďalších funkciách synchronizácie nájdete v téme Funkcie služby synchronizácie [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

