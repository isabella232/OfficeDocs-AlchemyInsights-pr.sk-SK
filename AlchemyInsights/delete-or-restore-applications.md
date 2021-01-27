---
title: Odstránenie alebo obnovenie aplikácií
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015016"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="d97b6-102">Odstránenie alebo obnovenie aplikácií</span><span class="sxs-lookup"><span data-stu-id="d97b6-102">Delete or restore applications</span></span>

<span data-ttu-id="d97b6-103">**Ak chcete odstrániť aplikáciu zo svojho nájomníka služby Azure AD**:</span><span class="sxs-lookup"><span data-stu-id="d97b6-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="d97b6-104">Na **portáli Azure AD** vyberte položku **podnikové aplikácie**.</span><span class="sxs-lookup"><span data-stu-id="d97b6-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="d97b6-105">Potom vyhľadajte aplikáciu, ktorú chcete odstrániť, a vyberte ju.</span><span class="sxs-lookup"><span data-stu-id="d97b6-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="d97b6-106">V časti **Spravovať** na ľavej table vyberte položku **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="d97b6-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="d97b6-107">Vyberte položku **odstrániť** a potom výberom položky **Áno** potvrďte, že chcete aplikáciu odstrániť zo svojho nájomníka služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d97b6-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="d97b6-108">Ďalšie informácie o odstránení aplikácie nájdete v téme rýchly štart [: odstránenie aplikácie z nájomníka služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="d97b6-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="d97b6-109">Rutina cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) v prostredí PowerShell odstraňuje konfigurácie aplikačných serverov proxy z konkrétnej aplikácie v službe Azure Active Directory a môže ju úplne odstrániť, ak je určená.</span><span class="sxs-lookup"><span data-stu-id="d97b6-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="d97b6-110">**Odstránenú aplikáciu môžete obnoviť** pomocou prostredia PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d97b6-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="d97b6-111">Po identifikácii aplikácie, ktorú chcete obnoviť, ju môžete obnoviť pomocou [obnovenia – AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="d97b6-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
