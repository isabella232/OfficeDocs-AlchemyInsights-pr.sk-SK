---
title: UPN synchronizácia zdravotne postihnutých
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921723"
---
# <a name="upn-sync-disabled"></a>UPN synchronizácia zdravotne postihnutých

Ak ste začali synchronizácii Azure AD pred marca 30, 2016, spustiť nasledovné cmdlet Azure AD PowerShell umožniť UPN mäkké zápas pre vašu organizáciu len:
  
 **Set-MsolDirSyncFeature-majú EnableSoftMatchOnUpn-povoliť $True**
  
UPN mäkké match sa automaticky zapne pre organizácie, ktoré začali synchronizácie s azúrovo reklamy alebo po marec 30, 2016.
  
Ďalšie informácie o zapnutí mäkké zápas na UPN a ďalšie funkcie synchronizácie, nájdete [Azure AD pripojiť funkcie synchronizácie služby](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

