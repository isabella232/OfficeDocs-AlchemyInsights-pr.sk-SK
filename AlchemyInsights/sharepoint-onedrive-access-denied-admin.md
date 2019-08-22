---
title: Riešenie problémov so správami prístup odmietnutý
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503554"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="0ff68-102">Riešenie problémov s prístup odmietnutý správy služby Sharepoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="0ff68-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="0ff68-103">Ak dostávate prístup odmietnutý správu pri pokuse vyhľadajte centrum správy služby Sharepoint/OneDrive, prosím uistite sa, že [Priradenie licencie k používateľovi](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="0ff68-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="0ff68-104">Ak používateľ nemá licenciu, tiež uistite, sú [priradenú rolu správcu](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , ktorá prístup admin centier.</span><span class="sxs-lookup"><span data-stu-id="0ff68-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="0ff68-105">Tento problém sa môže vyskytnúť aj pri používateľa sa odstráni a znova vytvorí s rovnaké hlavné meno používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="0ff68-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="0ff68-106">Nové konto je vytvorený pomocou rôznych PUID služby (Passport jedinečný identifikátor) hodnotu.</span><span class="sxs-lookup"><span data-stu-id="0ff68-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="0ff68-107">Keď sa používateľ pokúsi prístup kolekcie lokalít alebo ich OneDrive, používateľ má nesprávny PUID služby.</span><span class="sxs-lookup"><span data-stu-id="0ff68-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="0ff68-108">Druhý scenár zahŕňa adresár synchronizácia so Active Directory organizačnú jednotku (OU).</span><span class="sxs-lookup"><span data-stu-id="0ff68-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="0ff68-109">Ak používatelia už prihlásený do služby SharePoint, a potom sa presunie na rôznych OU a resynced so službou SharePoint, tento problém sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="0ff68-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="0ff68-110">Ak chcete vyriešiť tento problém, mali obnoviť pôvodný UPN s kroky v tomto článku, [obnovení používateľa v balíku Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="0ff68-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="0ff68-111">Poznámka: Ak OneDrive alebo SharePoint Admin center nie je k dispozícii pre viacerých používateľov, ktorí predtým prístup, môže byť problém pri dočasnej služby.</span><span class="sxs-lookup"><span data-stu-id="0ff68-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="0ff68-112">[Kontrola tabuľa stav služby](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="0ff68-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


