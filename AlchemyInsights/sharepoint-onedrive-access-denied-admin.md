---
title: Riešenie problémov s hlásením odmietnutia prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707969"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="7da63-102">Riešenie problémov s prístupom odmietnutých správ v centre spravovania SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="7da63-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="7da63-103">Ak sa pri pokuse o vyhľadanie v centre spravovania služby SharePoint/OneDrive zobrazuje hlásenie o odmietnutí prístupu, skontrolujte, či ste [používateľom priradili licenciu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="7da63-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="7da63-104">Ak má používateľ licenciu, mali by ste tiež uistiť, že im je [priradená rola správcu](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , ktorá môže získať prístup k centru spravovania.</span><span class="sxs-lookup"><span data-stu-id="7da63-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="7da63-105">Tento problém sa môže vyskytnúť aj po odstránení používateľa a opätovnom vytvorení s rovnakým hlavným menom používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="7da63-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="7da63-106">Nové konto sa vytvorí s použitím inej hodnoty PUID (jedinečného ID konta Passport).</span><span class="sxs-lookup"><span data-stu-id="7da63-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="7da63-107">Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo k ich OneDrivu, má používateľ nesprávny PUID.</span><span class="sxs-lookup"><span data-stu-id="7da63-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="7da63-108">Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="7da63-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="7da63-109">Ak sa používatelia už prihlásili do SharePointu a potom sa prenesú do inej OU a opätovne sa synchronizujú so SharePointom, tento problém sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="7da63-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="7da63-110">Ak chcete tento problém vyriešiť, mali by ste obnoviť pôvodné meno používateľa podľa krokov v článku a [obnoviť používateľa v službe Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="7da63-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="7da63-111">Poznámka: Ak centrum spravovania služby OneDrive alebo SharePoint nie je k dispozícii viacerým používateľom, ktorí mali predtým prístup, môže sa vyskytnúť dočasný problém so službou.</span><span class="sxs-lookup"><span data-stu-id="7da63-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="7da63-112">[Skontrolujte tabuľu stavu služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7da63-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


