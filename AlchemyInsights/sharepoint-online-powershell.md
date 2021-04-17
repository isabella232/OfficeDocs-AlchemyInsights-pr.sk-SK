---
title: Sharepoint Online PowerShell
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
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830597"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6ced2-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="6ced2-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6ced2-103">Pracujete s prostredím PowerShell alebo skriptmi v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="6ced2-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6ced2-104">Ďalšie informácie nájdete v prepojeniach nižšie.</span><span class="sxs-lookup"><span data-stu-id="6ced2-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6ced2-105">Začíname s prostrediami správy služby SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6ced2-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6ced2-106">Pripojenie k službe SPO pomocou viacfaktorového overovania (MFA)</span><span class="sxs-lookup"><span data-stu-id="6ced2-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6ced2-107">[SharePoint patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) (Vzory a postupy) obsahuje knižnicu príkazov prostredia PowerShell, ktorá umožňuje vykonávať komplexné akcie správy týkajúce sa služby SPO.</span><span class="sxs-lookup"><span data-stu-id="6ced2-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6ced2-108">Ak máte problémy s pripojením pomocou prostredia správy SPO, skontrolujte, či ste aktualizovali na najnovšiu verziu, a skúste znova [importovať modul](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) pomocou prostredia *Import-Module Microsoft.Online.SharePoint.PowerShell.*</span><span class="sxs-lookup"><span data-stu-id="6ced2-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6ced2-109">Ak sa pokúšate spustiť skripty objektového modelu na strane klienta, bude potrebné, aby bol v lokálnom počítači nainštalovaný softvér SDK pre klientske súčasti [SharePointu Online.](https://www.microsoft.com/download/details.aspx?id=42038)</span><span class="sxs-lookup"><span data-stu-id="6ced2-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6ced2-110">Ak máte problémy so spustením skriptov z prostredia PowerShell, môžete zvážiť spustenie prostredia PowerShell ako správca a zmenu [politiky spustenia.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="6ced2-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>