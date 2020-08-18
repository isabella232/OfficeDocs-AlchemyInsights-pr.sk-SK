---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786904"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="736bc-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="736bc-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="736bc-103">Pracujete s prostredím PowerShell alebo skriptami v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="736bc-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="736bc-104">Ďalšie informácie nájdete na prepojeniach nižšie.</span><span class="sxs-lookup"><span data-stu-id="736bc-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="736bc-105">Začíname so službou SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="736bc-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="736bc-106">Pripojenie k službe SPO PowerShell s overovaním multifacto (MFA)</span><span class="sxs-lookup"><span data-stu-id="736bc-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="736bc-107">[Šablóny a postupy SharePointu (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahujú knižnicu príkazov prostredia PowerShell, ktoré vám umožňujú vykonávať komplexné manažérske akcie na spo.</span><span class="sxs-lookup"><span data-stu-id="736bc-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="736bc-108">Ak máte problémy s pripojením k shellu riadenia SPO, uistite sa, že ste aktualizovali na najnovšiu verziu a pokúsite sa [znova importovať modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomocou *"Import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="736bc-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="736bc-109">Ak sa pokúšate spustiť skripty objektového modelu na strane klienta, bude potrebné, aby ste mali v lokálnom počítači nainštalovanú [súpravu SDK pre klientske súčasti SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="736bc-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="736bc-110">Ak máte problémy so spustením skriptov z prostredia PowerShell, môžete zvážiť spustenie prostredia PowerShell ako správca a zmeniť [politiku vykonávania](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="736bc-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>