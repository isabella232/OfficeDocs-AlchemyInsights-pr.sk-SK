---
title: UPN Sync zakázané
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726119"
---
# <a name="upn-sync-disabled"></a>UPN Sync zakázané

Ak ste spustili synchronizáciu Azure AD pred marec 30, 2016, spustite nasledujúce rutiny cmdlet Azure AD PowerShell umožniť UPN soft Match len pre vašu organizáciu:
  
 **Súbor MsolDirSyncFeature-funkcia EnableSoftMatchOnUpn-povoliť $True**
  
UPN soft Match je automaticky zapnutá pre organizácie, ktoré začali synchronizáciu Azure AD alebo po marec 30, 2016.
  
Ďalšie informácie o zapnutí funkcie soft Match v UPN a ďalších funkciách synchronizácie nájdete v časti [funkcie služby Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

