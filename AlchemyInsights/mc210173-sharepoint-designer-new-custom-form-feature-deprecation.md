---
title: MC210173 – Odstavenie novej funkcie vlastných formulárov pre SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831821"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="d883f-102">MC210173 – Odstavenie novej funkcie vlastných formulárov pre SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="d883f-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="d883f-103">Identifikovali sme problém, ktorý sa týka funkcií programu SharePoint Designer na [vytváranie vlastných formulárov](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) v SharePointe Online.</span><span class="sxs-lookup"><span data-stu-id="d883f-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="d883f-104">Po dôkladnom preskúmaní sme zistili, že na tento problém nie je známa žiadna oprava, a rozhodli sme sa vypnúť funkciu tvorby vlastných formulárov s účinnosťou od soboty 25. apríla 2020 o 3:00 UTC.</span><span class="sxs-lookup"><span data-stu-id="d883f-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="d883f-105">Táto zmena nemá vplyv na možnosť úprav predtým vytvorených formulárov alebo iné existujúce funkcie v službe SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="d883f-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="d883f-106">Po vykonaní tejto zmeny sa používateľom môže pri vytváraní nových formulárov zobraziť chybové hlásenie, že sa nepodarilo uložiť zoznam zmien na server.</span><span class="sxs-lookup"><span data-stu-id="d883f-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="d883f-107">Používatelia, ktorí už v minulosti využívali SharePoint Designer na tvorbu vlastných formulárov, budú môcť na tento účel namiesto toho využiť [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="d883f-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="d883f-108">PowerApps je jednoduchý a výkonný nástroj, ktorý umožňuje používateľom v modernom prostredí služby SharePoint Online vytvárať a upravovať vlastné formuláre pre zoznamy služby SharePoint a knižnice dokumentov priamo z okna prehliadača.</span><span class="sxs-lookup"><span data-stu-id="d883f-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="d883f-109">PowerApps nevyžaduje tradičné kódovacie znalosti, ani žiadne ďalšie stiahnuté aplikácie, ako je napríklad InfoPath.</span><span class="sxs-lookup"><span data-stu-id="d883f-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="d883f-110">**Poznámka**: Používatelia služby SharePoint Online v klasickom režime budú musieť dočasne prejsť na moderné prostredie, aby mohli využívať PowerApps. Všetky vlastné formuláre vytvorené v PowerApps sú však dostupné pre používateľov služby SharePoint Online v klasickom režime.</span><span class="sxs-lookup"><span data-stu-id="d883f-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
