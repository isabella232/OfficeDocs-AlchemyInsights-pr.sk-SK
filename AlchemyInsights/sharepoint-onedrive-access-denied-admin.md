---
title: Riešenie problémov s odmietnutým hlásením prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505394"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="dfc7a-102">Riešenie problémov s odmietnutým správam prístupu v Centre spravovania služby SharePoint alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="dfc7a-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="dfc7a-103">Ak pri pokuse o prehľadávanie Centra spravovania služby Sharepoint/OneDrive sa zobrazí hlásenie o odmietnutí prístupu, uistite sa, že [používateľovi priradíte licenciu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="dfc7a-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="dfc7a-104">Ak má používateľ licenciu, mali by ste sa tiež uistiť, že im bude [priradená rola správcu,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ktorá má prístup k centrám spravovania.</span><span class="sxs-lookup"><span data-stu-id="dfc7a-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="dfc7a-105">Tento problém sa môže vyskytnúť aj pri odstránení používateľa a znova vytvorené s rovnakým hlavným menom používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="dfc7a-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="dfc7a-106">Nové konto sa vytvorí pomocou inej hodnoty PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="dfc7a-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="dfc7a-107">Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo onedrive, používateľ má nesprávne PUID.</span><span class="sxs-lookup"><span data-stu-id="dfc7a-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="dfc7a-108">Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="dfc7a-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="dfc7a-109">Ak sa používatelia už prihlásili do služby SharePoint a potom sa premiestnia do inej ou a znova synchronizujú so službou SharePoint, môžu sa vyskytnúť tento problém.</span><span class="sxs-lookup"><span data-stu-id="dfc7a-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="dfc7a-110">Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN s krokmi v článku [Obnoviť používateľa v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="dfc7a-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="dfc7a-111">Poznámka: Ak OneDrive alebo SharePoint Admin Center nie je k dispozícii pre viacerých používateľov, ktorí predtým mali prístup, môže ísť o dočasný problém služby.</span><span class="sxs-lookup"><span data-stu-id="dfc7a-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="dfc7a-112">[Skontrolujte tabuľu stavu služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="dfc7a-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


