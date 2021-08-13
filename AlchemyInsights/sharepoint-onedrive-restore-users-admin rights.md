---
title: Riešenie problémov s hlásením o odmietnutí prístupu OneDrive for Business lokalitám
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957808"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Riešenie problémov s hlásením o odmietnutí prístupu OneDrive for Business lokalitám

Tento problém sa najčastejšie vyskytuje pri odstránení a vytvorení používateľa s rovnakým hlavným menom používateľa (UPN). Nové konto sa vytvorí pomocou inej hodnoty PUID (Passport Unique ID). Keď sa používateľ pokúsi získať prístup ku kolekcii lokalít alebo OneDrive, používateľovi sa zobrazí nesprávna identifikácia PUID. Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory. Ak sa používatelia už prihlásili do služby SharePoint a potom sa presunú do inej poštovej schránky a znova synchronizujú s SharePoint, môže sa im zobraziť tento problém.

1. Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné používateľské meno používateľa pomocou krokov uvedených v článku [Obnovenie používateľa v Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Ak nie je možné obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z lokality OneDrive pomocou týchto krokov Odstrániť používateľa [zo zoznamu informácií o používateľoch.]() 
3. Po dokončení tohto postupu môžete overiť, či má používateľ práva správcu na lokalitu OneDrive pomocou krokov na pridanie správcu pre [používateľove OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Ďalšie informácie o úrovniach povolení nájdete v článku Úrovne [povolení v SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
