---
title: Odstránenie služby na pozadí pre Microsoft Search v službe Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816337"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="85500-102">Odstránenie služby na pozadí pre Microsoft Search v službe Bing</span><span class="sxs-lookup"><span data-stu-id="85500-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="85500-103">Ak chcete odstrániť službu na pozadí pre Microsoft Search v službe Bing, môžete vyskúšať tieto opravné prostriedky:</span><span class="sxs-lookup"><span data-stu-id="85500-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="85500-104">Ak sa chcete vrátiť k pôvodnému nastaveniu vyhľadávacieho nástroja, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="85500-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="85500-105">a.</span><span class="sxs-lookup"><span data-stu-id="85500-105">a.</span></span> <span data-ttu-id="85500-106">Prepnutie na prepínač **použiť Bing ako predvolený vyhľadávací [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) nástroj je vypnutý**.</span><span class="sxs-lookup"><span data-stu-id="85500-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="85500-107">b.</span><span class="sxs-lookup"><span data-stu-id="85500-107">b.</span></span> <span data-ttu-id="85500-108">[Prejdite do centra spravovania služieb Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) a zrušte začiarknutie nastavenia, ktoré ovplyvní všetkých používateľov vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="85500-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="85500-109">Ak chcete odstrániť službu na pozadí z jedného zariadenia, vykonajte tieto úlohy:</span><span class="sxs-lookup"><span data-stu-id="85500-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="85500-110">a.</span><span class="sxs-lookup"><span data-stu-id="85500-110">a.</span></span> <span data-ttu-id="85500-111">Vyberte položku **Ovládací Panel > programy > programy a súčasti**.</span><span class="sxs-lookup"><span data-stu-id="85500-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="85500-112">b.</span><span class="sxs-lookup"><span data-stu-id="85500-112">b.</span></span> <span data-ttu-id="85500-113">Kliknite pravým tlačidlom myši na položku **Microsoft Search v Bingu** v zozname nainštalovaných programov a potom kliknite na položku **odinštalovať**.</span><span class="sxs-lookup"><span data-stu-id="85500-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="85500-114">Ak chcete odstrániť službu na pozadí z viacerých zariadení vo vašej organizácii, prihláste sa ako správca a v skripte spustite nasledujúci príkaz:</span><span class="sxs-lookup"><span data-stu-id="85500-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
