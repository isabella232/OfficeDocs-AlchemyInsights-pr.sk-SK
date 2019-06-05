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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719496"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Vytvorenie skupiny pripojené lokality SharePoint Online

<p><strong>Existuje niekoľko spoločných otázok sa vyskytla vytvorenie alebo re-vytvárať skupinu pripojení stránky.&nbsp;</strong></p>  <p>1.Ak ste odstránili skupine a jej prepojené stránky a chcete vytvoriť inú stránku s rovnakou adresou URL, musíte natrvalo odstrániť predchádzajúcu stránku.</p>  <ul>  <li>Stiahnuť <a title="SPO Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - viac info na Začíname s powershell nájdete <a title="Začíname s SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Začíname s SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Odstránenie lokality z lokality odstránené pomocou <a title="odstrániť SPODeletedSiteSharePoint" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Odstrániť-SPODeletedSiteSharePoint</a> cmdlet prostredia powershell.</li>  </ul>  <p>Ak vytvárate skupina prepojených stránok a prijímať upozornenia <strong>"inej skupiny s rovnakým aliasu už existuje"</strong>, skontrolujte existujúce skupiny z <a title="Office 365 Admin Center" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 Admin Center</a>. Ak chcete vyriešiť problém, ak už nie je potrebné odstrániť existujúcu skupinu alebo vytvoríte stránky s rozdielnymi aliasmi pridelené.&nbsp;</p>  <p><strong>Existujú rôzne spôsoby, ako vytvoriť a používať moderné skupiny so službou SharePoint.&nbsp;</strong></p>  <ol>  <li>Existujúce lokality môžete pripojiť do skupiny Office 365. Ďalšie informácie nájdete v téme <a title="pripojiť skupiny Office 365 pomocou SharePoint používateľa ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Pripojiť skupiny Office 365 pomocou SharePoint používateľa ineterface</a>.</li>  <li>Ak chcete vytvoriť lokalitu Office 365 skupiny pripojené, budete musieť vytvoriť lokalitu tímu. Ďalšie informácie nájdete v téme <a title="vytvorenie tímovej lokality SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Vytvorenie tímovej lokality SharePoint.</a></li>  </ol>

