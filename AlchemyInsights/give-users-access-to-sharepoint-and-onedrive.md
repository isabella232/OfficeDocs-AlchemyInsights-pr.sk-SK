---
title: Udelenie prístupu používateľom k SharePointu a OneDrivu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677222"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="42b2b-102">Udelenie prístupu používateľom k SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="42b2b-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="42b2b-103">Ak OneDrive alebo SharePoint nie je k dispozícii viacerým používateľom, ktorí mali predtým prístup, môže sa vyskytnúť dočasný problém so službou.</span><span class="sxs-lookup"><span data-stu-id="42b2b-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="42b2b-104">Kontrola tabule stavu služby</span><span class="sxs-lookup"><span data-stu-id="42b2b-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="42b2b-105">Ak chcete, aby sa ľudia vo vašej organizácii mohli prihlásiť a používať SharePoint a OneDrive, musíte k nim pridať kontá a uistiť sa, že majú licenciu, ktorá im umožní prístup k SharePointu a OneDrivu.</span><span class="sxs-lookup"><span data-stu-id="42b2b-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="42b2b-106">Najjednoduchším spôsobom, ako pridať používateľov, je v centre spravovania služieb Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="42b2b-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="42b2b-107">Prejdite na [stránku aktívni používatelia v centre spravovania služieb Microsoft 365](https://portal.office.com/adminportal/home#/users)a potom kliknite na položku **Pridať používateľa**.</span><span class="sxs-lookup"><span data-stu-id="42b2b-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="42b2b-108">Vyplňte informácie pre používateľa a skontrolujte, či je v časti licencie na **produkt**priradená licencia a či je vybratá možnosť **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="42b2b-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="42b2b-109">Ak v organizácii povolíte externé zdieľanie, používatelia môžu zdieľať obsah SharePointu a OneDrivu s ľuďmi mimo organizácie.</span><span class="sxs-lookup"><span data-stu-id="42b2b-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="42b2b-110">Nemusíte poskytnúť týmto externým používateľom licencie.</span><span class="sxs-lookup"><span data-stu-id="42b2b-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="42b2b-111">Ak nie je zdieľanie nastavené na možnosť len existujúci Externí používatelia, nie je potrebné pridať k nim kontá.</span><span class="sxs-lookup"><span data-stu-id="42b2b-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="42b2b-112">Ak sa v tomto prípade ľudia nenachádzajú v adresári vašej organizácie, musíte ich pridať ako hosťujúci používatelia v centre spravovania služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="42b2b-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

