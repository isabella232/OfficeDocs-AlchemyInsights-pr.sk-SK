---
title: Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232554"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality

Tento problém sa vyskytuje najčastejšie keď používateľ odstráni a znova vytvorí s rovnaké hlavné meno používateľa (UPN). Nové konto je vytvorený pomocou rôznych PUID služby (Passport jedinečný identifikátor) hodnotu. Keď sa používateľ pokúsi prístup kolekcie lokalít alebo ich OneDrive, používateľ má nesprávny PUID služby. Druhý scenár zahŕňa adresár synchronizácia so Active Directory organizačnú jednotku (OU). Ak používatelia už prihlásený do služby SharePoint, a potom sa presunie na rôznych OU a resynced so službou SharePoint, tento problém sa môže vyskytnúť.

1. Na vyriešenie tohto problému by ste mali obnoviť pôvodný UPN s kroky v tomto článku,[obnovení používateľa v balíku Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ak nemôžete obnoviť pôvodný používateľ mali odstrániť starý používateľské z OneDrive stránky pomocou týchto krokov, [Odstránenie používateľa zo zoznamu používateľov info](). 
3. Po sa to deje, môžete si overiť má používateľ admin práva na OneDrive stránky pomocou nasledujúcich krokov na [Pridanie admin's používateľa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Ďalšie informácie o úrovniach povolení nájdete v článku [pochopenie úrovne povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
