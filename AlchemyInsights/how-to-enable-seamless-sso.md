---
title: Povolenie bezproblémového SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780542"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="82ba6-102">Povolenie bezproblémového SSO</span><span class="sxs-lookup"><span data-stu-id="82ba6-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="82ba6-103">Povoliť bezproblémové SSO prostredníctvom služby [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="82ba6-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="82ba6-104">Ak vytvárate novú inštaláciu služby Azure AD Connect, vyberte [vlastnú cestu inštalácie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="82ba6-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="82ba6-105">Na **prihlasovacej stránke používateľa** vyberte možnosť **Povoliť jediné prihlásenie** .</span><span class="sxs-lookup"><span data-stu-id="82ba6-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="82ba6-106">Ak chcete overiť, či ste správne povolili bezproblémové prihlásenie:</span><span class="sxs-lookup"><span data-stu-id="82ba6-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="82ba6-107">Prihláste sa do [centra spravovania služby Azure Active Directory](https://aad.portal.azure.com) ako globálny správca.</span><span class="sxs-lookup"><span data-stu-id="82ba6-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="82ba6-108">Na ľavej table vyberte položku **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="82ba6-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="82ba6-109">Overte, či je **zapnuté**bezproblémové jediné prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="82ba6-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="82ba6-110">Ďalšie informácie nájdete v téme [jednoduché prihlásenie v službe Azure Active Directory: rýchly začiatok](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="82ba6-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  