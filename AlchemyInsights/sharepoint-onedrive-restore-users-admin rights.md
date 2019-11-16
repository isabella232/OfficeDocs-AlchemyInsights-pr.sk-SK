---
title: Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766726"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality

Tento problém sa vyskytuje najčastejšie pri odstránení používateľa a znova vytvoriť s rovnakým hlavným menom používateľa (UPN). Nový účet je vytvorený pomocou iného PUID (Passport unique ID) hodnotu. Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo ich OneDrive, používateľ má nesprávne PUID. Druhý scenár zahŕňa synchronizáciu adresárov s Active Directory organizačnú jednotku (OU). Ak používatelia už prihlásení do služby SharePoint a potom sa premiestnia do iného OU a resynced s SharePoint, môžu sa vyskytnúť tento problém.

1. Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN kroky v článku, [obnovenie používateľa v balíku Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ak nemôžete obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z OneDrive stránky pomocou týchto krokov, [odstrániť používateľa zo zoznamu informácie o používateľovi](). 
3. Po dokončení tohto postupu môžete overiť, že používateľ má administrátorské práva na lokalitu OneDrive podľa krokov na [Pridanie admin pre používateľa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Ďalšie informácie o úrovniach povolení nájdete [v článku Vysvetlenie úrovní povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
