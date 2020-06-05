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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582826"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problémy pri vytváraní skupiny pripojenej lokality v SharePointe

1. Pri vytváraní alebo opätovnom vytváraní skupiny pripojenej lokality sa vyskytli problémy.
Ak ste odstránili skupinu a jej pripojenú lokalitu a chcete vytvoriť inú lokalitu s rovnakou adresou URL, budete musieť natrvalo odstrániť predchádzajúcu lokalitu.

   - Stiahnuť [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Ďalšie informácie o tom, ako začať pracovať s powershellom, nájdete v téme [Začíname pracovať s prostredím správy SharePointu Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Odstránenie lokality z odstránených lokalít pomocou rutiny cmdlet prostredia Powershell [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell je potrebné natrvalé odstránenie skupiny lokalít.

1. Ak vytvárate skupinu pripojenú lokalitu a zobrazí sa upozornenie: **Ďalšia skupina s rovnakým aliasom už existuje,** skontrolujte existujúce skupiny z Centra spravovania služby [Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Ak chcete vyriešiť tento problém, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.

1. Existujú rôzne spôsoby vytvárania a používania moderných skupín so SharePointom.

   - Existujúce lokality môžete pripojiť k skupine Microsoft 365. Ďalšie informácie nájdete v téme [Pripojenie skupiny Microsoft 365 pomocou používateľského rozhrania SharePointu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Ak chcete vytvoriť pripojenú lokalitu skupiny Microsoft 365, musíte vytvoriť [tímovú lokalitu](https://admin.microsoft.com/sharepoint).
