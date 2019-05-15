---
title: Moderné lokalitu ako root
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057771"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="0ca07-102">Moderné lokalitu ako root</span><span class="sxs-lookup"><span data-stu-id="0ca07-102">Modern site as root site</span></span>

<span data-ttu-id="0ca07-103">[Cieľ uvoľnenia](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) zákazníci teraz umožňujú moderné komunikačné stránky skúsenosti v klasickej koreňovej lokality zemepána SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ca07-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="0ca07-104">Túto funkciu možno aktivovať jednoduché rutiny cmdlet prostredia PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0ca07-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="0ca07-105">Na úspešnú realizáciu PowerShell Command (s), koreňovej lokality bude mať novú komunikáciu stránky domovskú stránku.</span><span class="sxs-lookup"><span data-stu-id="0ca07-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="0ca07-106">Podrobnosti o požiadavkách na PowerShell cmdlet a funkcie sú k dispozícii v článku [Povoliť-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="0ca07-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="0ca07-107">Budeme postupne kymácení, off predvolene cielené uvoľnenie zákazníkom v začiatkom mája 2019 a dojazdu bude k dispozícii po celom svete do konca júna 2019.</span><span class="sxs-lookup"><span data-stu-id="0ca07-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="0ca07-108">Naďalej odkazovať [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) pre ďalšie nové funkcie s moderným.</span><span class="sxs-lookup"><span data-stu-id="0ca07-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="0ca07-109">**Dôležité**: Neodstraňujte klasickej koreňovej lokality vytvoriť lokalitu modernej komunikácie.</span><span class="sxs-lookup"><span data-stu-id="0ca07-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="0ca07-110">To nie je podporovaný spoločnosťou Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0ca07-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="0ca07-111">Odstránenie koreňovej lokality bude všetkých lokalít SharePoint vo vašej organizácii neprístupné pre všetkých užívateľov, kým obnovenie lokality alebo vytvoriť novú lokalitu na rovnakú adresu URL.</span><span class="sxs-lookup"><span data-stu-id="0ca07-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 