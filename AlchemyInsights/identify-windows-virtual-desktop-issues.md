---
title: Identifikácia problémov týkajúcich sa virtuálnej pracovnej plochy Windowsu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596040"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="79b66-102">Identifikácia problémov týkajúcich sa virtuálnej pracovnej plochy Windowsu</span><span class="sxs-lookup"><span data-stu-id="79b66-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="79b66-103">Diagnostika virtuálnej pracovnej plochy systému Windows používa iba jednu rutinu typu cmdlet prostredia PowerShell, no obsahuje mnoho voliteľných parametrov, ktoré vám pomôžu určiť a určiť problémy.</span><span class="sxs-lookup"><span data-stu-id="79b66-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="79b66-104">Začíname:</span><span class="sxs-lookup"><span data-stu-id="79b66-104">To get started:</span></span> 

1. <span data-ttu-id="79b66-105">Stiahnite a importujte modul Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="79b66-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="79b66-106">Podrobnosti nájdete v téme [Rutiny typu cmdlet virtuálnej pracovnej plochy Windowsu pre Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="79b66-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="79b66-107">Na prihlásenie do konta spustite nasledujúcu rutinu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="79b66-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="79b66-108">Príklad: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="79b66-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="79b66-109">**POZNÁMKA:** Všetky dotazy používajúce prostredie PowerShell musia obsahovať parametre -UserName alebo -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="79b66-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="79b66-110">Informácie o možnostiach sledovania nájdete v téme [Používanie analýzy denníka pre diagnostické funkcie.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="79b66-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="79b66-111">Ak chcete filtrovať diagnostické aktivity podľa používateľa, spustite nasledujúcu rutinu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="79b66-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="79b66-112">Príklad: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="79b66-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="79b66-113">K dispozícii je zoznam filtrov, pomocou ktorých môžete diagnostikovať problémy.</span><span class="sxs-lookup"><span data-stu-id="79b66-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="79b66-114">Ďalšie informácie o diagnostike problémov nájdete v téme Identifikácia a [diagnostika problémov virtuálnej pracovnej plochy Windowsu.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="79b66-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="79b66-115">Ďalšie informácie o bežných chybách nájdete v [téme Bežné chyby ako šucháky](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="79b66-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
