---
title: Pridanie skupiny na SharePoint lokalitu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897731"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Bežné problémy pri vytváraní lokality pripojenej ku skupine v SharePoint

1. Ak ste odstránili skupinu a pripojenú lokalitu a chcete vytvoriť ďalšiu lokalitu s rovnakou URL adresou, budete musieť predchádzajúcu lokalitu natrvalo odstrániť.

   - Stiahnuť [prostredie správy SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Ďalšie informácie o tom, ako začať pracovať s prostredím PowerShell, nájdete v téme [Začíname pracovať SharePoint prostredím Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Odstráňte lokalitu z odstránených lokalít pomocou rutiny typu cmdlet prostredia Powershell [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Na trvalé odstránenie skupinových lokalít sa vyžaduje prostredie PowerShell.

1. Ak vytvárate pripojenú lokalitu skupiny a zobrazí sa upozornenie: Iná skupina s rovnakým **aliasom** už existuje, skontrolujte existujúce skupiny z [Centrum spravovania služby Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Ak chcete tento problém vyriešiť, odstráňte existujúcu skupinu, ak už nie je potrebná, alebo vytvorte lokalitu s iným priradeným aliasom.

1. Existujú rôzne spôsoby, ako vytvoriť a používať moderné skupiny s SharePoint.

   - Môžete pripojiť existujúce lokality k Microsoft 365 skupine. Ďalšie informácie nájdete v [Pripojenie skupiny Microsoft 365 pomocou používateľského SharePoint rozhrania](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Ak chcete Microsoft 365 pripojenú lokalitu pre inú skupinu, musíte vytvoriť [tímovú lokalitu.](https://admin.microsoft.com/sharepoint)
