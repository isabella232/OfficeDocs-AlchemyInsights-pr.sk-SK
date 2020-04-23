---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764276"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="c9724-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="c9724-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="c9724-103">Práca s PowerShell alebo skripty v rámci SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="c9724-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="c9724-104">Ďalšie informácie nájdete na nižšie uvedených odkazoch.</span><span class="sxs-lookup"><span data-stu-id="c9724-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="c9724-105">Začíname pracovať s SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="c9724-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="c9724-106">Pripojenie k SPO PowerShell s multifaktorové overovanie (MFA)</span><span class="sxs-lookup"><span data-stu-id="c9724-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="c9724-107">[SharePoint vzory a postupy (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahuje knižnicu príkazov PowerShell, ktoré vám umožní vykonávať komplexné riadenie činnosti voči spo.</span><span class="sxs-lookup"><span data-stu-id="c9724-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="c9724-108">Ak máte problémy s pripojením k správe SPO Management Shell, uistite sa, že ste aktualizovali na najnovšiu verziu a pokúste sa [znova importovať modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomocou *"Import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="c9724-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="c9724-109">Ak sa pokúšate spustiť klientske skripty objektového modelu, budete musieť mať [SharePoint Online client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) nainštalovaný na lokálnom počítači.</span><span class="sxs-lookup"><span data-stu-id="c9724-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="c9724-110">Ak máte problémy so spustením skriptov z PowerShell, možno budete chcieť zvážiť spustenie PowerShell ako správca a zmena [vykonávania politiky](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="c9724-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>