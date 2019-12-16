---
title: Pridanie skupiny na lokalitu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051116"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problémy pri vytváraní alebo zoskupovanie pripojených lokalít SharePoint Online

Existuje niekoľko bežných problémov, ktoré sa vyskytli pri vytváraní alebo opätovnom vytvorení skupiny pripojenej lokality.

 Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou webovou adresou, musíte natrvalo odstrániť predchádzajúcu lokalitu.

Na stiahnutie [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Ďalšie informácie o Začíname s PowerShell, pozrite si Začíname [s SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Odstráňte lokalitu z odstránených lokalít pomocou rutiny cmdlet prostredia PowerShell [odstrániť SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Ak vytvárate skupinu pripojenú lokalitu a prijmete upozornenie, ďalšia skupina s rovnakým aliasom už existuje, skontrolujte existujúce skupiny z [balíka Office 365 z centra spravovania](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Ak chcete vyriešiť tento problém, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.

Existujú rôzne spôsoby vytvárania a používania moderných skupín so službou SharePoint.

Existujúce lokality môžete pripojiť k skupine Office 365. Ďalšie informácie nájdete v téme [pripojenie skupiny Office 365 pomocou používateľa služby SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Ak chcete vytvoriť lokalitu Connected Office 365 Group, musíte vytvoriť tímovú lokalitu. Ďalšie informácie nájdete v téme [vytvorenie tímovej lokality v službe SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

