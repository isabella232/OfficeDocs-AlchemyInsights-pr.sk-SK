---
title: Pridať skupinu lokality SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507862"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problémy pri vytváraní alebo skupiny pripojený lokality SharePoint Online

Existuje niekoľko spoločných otázok sa vyskytla vytvorenie alebo re-vytvárať skupinu pripojení stránky.

 Ak ste odstránili skupine a jej prepojené stránky a chcete vytvoriť inú stránku s rovnakou adresou URL, musíte natrvalo odstrániť predchádzajúcu stránku.

Stiahnuť [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Viac info na Začíname s powershell v téme [Začíname pracovať s SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Odstránenie lokality zo odstránené lokalít pomocou rutiny cmdlet [Remove-SPODeletedSiteSharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) prostredia powershell.

Ak vytvárate skupina prepojených stránok a upozornení, iné skupiny s rovnakým aliasu už existuje, skontrolujte, či existujúce skupiny z [Office 365 Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Ak chcete vyriešiť problém, ak už nie je potrebné odstrániť existujúcu skupinu alebo vytvoríte stránky s rozdielnymi aliasmi pridelené.

Existujú rôzne spôsoby, ako vytvoriť a používať moderné skupiny so službou SharePoint.

Existujúce lokality môžete pripojiť do skupiny Office 365. Ďalšie informácie nájdete v téme [pripojenie skupiny Office 365 pomocou SharePoint používateľa ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Ak chcete vytvoriť lokalitu Office 365 skupiny pripojené, budete musieť vytvoriť lokalitu tímu. Ďalšie informácie nájdete v téme [vytvorenie tímovej lokality SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

