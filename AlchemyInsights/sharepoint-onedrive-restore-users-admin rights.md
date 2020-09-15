---
title: Riešenie problémov s prístupom odmietnutých správ na lokality služby OneDrive for Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670631"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Riešenie problémov s prístupom odmietnutých správ na lokality služby OneDrive for Business

Tento problém sa vyskytuje najčastejšie pri odstránení používateľa a opätovnom vytvorení s rovnakým hlavným menom používateľa (UPN). Nové konto sa vytvorí s použitím inej hodnoty PUID (jedinečného ID konta Passport). Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo k ich OneDrivu, má používateľ nesprávny PUID. Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU). Ak sa používatelia už prihlásili do SharePointu a potom sa prenesú do inej OU a opätovne sa synchronizujú so SharePointom, tento problém sa môže vyskytnúť.

1. Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné meno používateľa podľa krokov v článku [obnovenie používateľa v programe Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ak nie je možné obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z lokality OneDrive pomocou týchto krokov, [odstrániť používateľa zo zoznamu informácie o používateľoch](). 
3. Po dokončení tohto postupu môžete overiť, či má používateľ práva správcu na lokalitu OneDrive, a to pomocou krokov na [Pridanie správcu pre OneDrive používateľa](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Ďalšie informácie o úrovniach povolení nájdete v článku [Vysvetlenie úrovní povolení v SharePointe](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
