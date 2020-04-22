---
title: Riešenie problémov s odmietané správy programu Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758512"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Riešenie problémov s odmietané správy v službe SharePoint/OneDrive admin Center

Ak sa pri pokuse o prehľadávanie do centra spravovania služby SharePoint/OneDrive zobrazí hlásenie o odmietnutí prístupu, uistite sa, že ste [používateľovi priradili licenciu](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ak má používateľ licenciu, mali by ste sa tiež uistiť, že sú [priradené rolu správcu](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , ktorá má prístup do centra spravovania.

Tento problém sa môže vyskytnúť aj pri odstránení používateľa a znova vytvoriť s rovnakým hlavným menom používateľa (UPN). Nový účet je vytvorený pomocou iného PUID (Passport unique ID) hodnotu. Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo ich OneDrive, používateľ má nesprávne PUID. Druhý scenár zahŕňa synchronizáciu adresárov s Active Directory organizačnú jednotku (OU). Ak používatelia už prihlásení do služby SharePoint a potom sa premiestnia do iného OU a resynced s SharePoint, môžu sa vyskytnúť tento problém.

Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN kroky v článku, [obnovenie používateľa v Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Poznámka: Ak OneDrive alebo SharePoint admin Center nie je k dispozícii viacerým používateľom, ktorí predtým mali prístup, môže existovať dočasný problém služby.  [Skontrolujte stav služby tabuľa](https://portal.office.com/adminportal/home#/servicehealth).


