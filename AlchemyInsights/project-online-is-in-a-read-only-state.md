---
title: Project Online je v stave iba na čítanie
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801667"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="db381-102">Project Online je v stave iba na čítanie</span><span class="sxs-lookup"><span data-stu-id="db381-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="db381-103">Existujú tri bežné dôvody, prečo Project Online môže dosiahnuť stav iba na čítanie:</span><span class="sxs-lookup"><span data-stu-id="db381-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="db381-104">Organizácie majú iba licencie na Project Online Essentials.</span><span class="sxs-lookup"><span data-stu-id="db381-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="db381-105">Toto nestačí na to, aby sa lokalita nachádzala nažive a nakoniec sa obmedzila.</span><span class="sxs-lookup"><span data-stu-id="db381-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="db381-106">Lokalita sa umiestni v stave iba na čítanie, aby správcovia vedeli, že je niečo zle a môže získať správne licencie.</span><span class="sxs-lookup"><span data-stu-id="db381-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="db381-107">Správcovia budú musieť pridať licenciu na Project Online Professional alebo Premium.</span><span class="sxs-lookup"><span data-stu-id="db381-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="db381-108">Lokalita bude z tohto miesta vychádzať iba na čítanie.</span><span class="sxs-lookup"><span data-stu-id="db381-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="db381-109">Ďalšie informácie nájdete v téme [porovnanie riešení na riadenie projektov](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="db381-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="db381-110">Dosiahla sa priradená kvóta.</span><span class="sxs-lookup"><span data-stu-id="db381-110">Assigned quota has been reached.</span></span> <span data-ttu-id="db381-111">Ďalšie informácie nájdete v téme [kvóta webovej aplikácie Project Web App](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="db381-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="db381-112">Ak chcete zistiť, ako môže zrnitosť zostavy ovplyvniť používanie kvóty, začiarknite políčko [Konfigurovať súhrn údajov s časovým usporiadaním údajov v Projecte Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) .</span><span class="sxs-lookup"><span data-stu-id="db381-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="db381-113">Iba na čítanie môže byť veľmi dočasná podmienka, ktorá sa môže vyskytnúť počas údržby.</span><span class="sxs-lookup"><span data-stu-id="db381-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="db381-114">Väčšina údržby si ani nevšimol naši zákazníci a nebudete ju často vidieť, ale sú chvíle, kedy sa vyskytli krátke obdobia iba na čítanie.</span><span class="sxs-lookup"><span data-stu-id="db381-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
