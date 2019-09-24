---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123013"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="953e0-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="953e0-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="953e0-103">Práca s PowerShell alebo skripty v rámci SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="953e0-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="953e0-104">Ďalšie informácie nájdete na nižšie uvedených odkazoch.</span><span class="sxs-lookup"><span data-stu-id="953e0-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="953e0-105">Začíname pracovať s SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="953e0-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="953e0-106">Pripojenie k SPO PowerShell s multifaktorové overovanie (MFA)</span><span class="sxs-lookup"><span data-stu-id="953e0-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="953e0-107">[SharePoint vzory a postupy (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahuje knižnicu príkazov PowerShell, ktoré vám umožní vykonávať komplexné riadenie činnosti voči spo.</span><span class="sxs-lookup"><span data-stu-id="953e0-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="953e0-108">Ak máte problémy s pripojením k správe SPO Management Shell, uistite sa, že ste aktualizovali na najnovšiu verziu a pokúste sa [znova importovať modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomocou *"Import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="953e0-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="953e0-109">Ak sa pokúšate spustiť klientske skripty objektového modelu, budete musieť mať [SharePoint Online client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) nainštalovaný na lokálnom počítači.</span><span class="sxs-lookup"><span data-stu-id="953e0-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="953e0-110">Ak máte problémy so spustením skriptov z PowerShell, možno budete chcieť zvážiť spustenie PowerShell ako správca a zmena [vykonávania politiky](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="953e0-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>