---
title: Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692816"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality

Tento problém sa vyskytuje najčastejšie pri odstránení používateľa a znova vytvoriť s rovnakým hlavným menom používateľa (UPN). Nový účet je vytvorený pomocou iného PUID (Passport unique ID) hodnotu. Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo ich OneDrive, používateľ má nesprávne PUID. Druhý scenár zahŕňa synchronizáciu adresárov s Active Directory organizačnú jednotku (OU). Ak používatelia už prihlásení do služby SharePoint a potom sa premiestnia do iného OU a resynced s SharePoint, môžu sa vyskytnúť tento problém.

1. Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN kroky v článku, [obnovenie používateľa v Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ak nemôžete obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z OneDrive stránky pomocou týchto krokov, [odstrániť používateľa zo zoznamu informácie o používateľovi](). 
3. Po dokončení tohto postupu môžete overiť, že používateľ má administrátorské práva na lokalitu OneDrive podľa krokov na [Pridanie admin pre používateľa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Ďalšie informácie o úrovniach povolení nájdete [v článku Vysvetlenie úrovní povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
