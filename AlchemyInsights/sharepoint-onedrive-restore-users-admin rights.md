---
title: Riešenie problémov s prístupom odmietnutýsprávy onedrive business lokality
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511199"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Riešenie problémov s prístupom odmietnutýsprávy onedrive business lokality

Tento problém sa najčastejšie vyskytuje, keď sa používateľ odstráni a znova vytvorí s rovnakým hlavným menom používateľa (UPN). Nové konto sa vytvorí pomocou inej hodnoty PUID (Passport Unique ID). Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo onedrive, používateľ má nesprávne PUID. Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU). Ak sa používatelia už prihlásili do služby SharePoint a potom sa premiestnia do inej ou a znova synchronizujú so službou SharePoint, môžu sa vyskytnúť tento problém.

1. Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN s krokmi v článku [Obnoviť používateľa v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ak nemôžete obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z lokality OneDrive pomocou týchto krokov, [Odstráňte používateľa zo zoznamu informácií o používateľovi](). 
3. Po vykonaní tohto postupu môžete overiť, že používateľ má práva správcu na lokalitu OneDrive podľa krokov na [pridanie správcu pre používateľa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Ďalšie informácie o úrovniach povolení nájdete v článku [Informácie o úrovniach povolení v SharePointe](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
