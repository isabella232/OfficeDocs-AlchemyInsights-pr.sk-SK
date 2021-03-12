---
title: Riešenie problémov s inštaláciou MDATP v Macu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749769"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="e93a0-102">Riešenie problémov s inštaláciou MDATP v Macu</span><span class="sxs-lookup"><span data-stu-id="e93a0-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="e93a0-103">Ak manuálna inštalácia zlyhá, **súhrnná** stránka Sprievodcu inštaláciou zobrazí sa nasledujúca chyba:</span><span class="sxs-lookup"><span data-stu-id="e93a0-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="e93a0-104">Počas inštalácie sa vyskytla chyba.</span><span class="sxs-lookup"><span data-stu-id="e93a0-104">"An error occurred during installation.</span></span> <span data-ttu-id="e93a0-105">Inštalátor zistil chybu, ktorá spôsobila zlyhanie inštalácie.</span><span class="sxs-lookup"><span data-stu-id="e93a0-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="e93a0-106">Požiadajte o pomoc výrobcu softvéru.</span><span class="sxs-lookup"><span data-stu-id="e93a0-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="e93a0-107">Pri nasadení MDM sa na stránke zobrazuje zlyhanie všeobecného inštalácie.</span><span class="sxs-lookup"><span data-stu-id="e93a0-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="e93a0-108">Hoci sa na koncových používateľov nezobrazujú presné chyby, v **/Library/logs/Microsoft/mdatp/Install.log** sa uchová súbor denníka s priebehom inštalácie.</span><span class="sxs-lookup"><span data-stu-id="e93a0-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="e93a0-109">Každá relácia inštalácie sa pridá do tohto súboru denníka.</span><span class="sxs-lookup"><span data-stu-id="e93a0-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="e93a0-110">Ak chcete použiť len poslednú reláciu inštalácie, použite `sed` .</span><span class="sxs-lookup"><span data-stu-id="e93a0-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="e93a0-111">Ďalšie informácie nájdete v téme [Riešenie problémov s inštaláciou programu Microsoft Defender ATP pre Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="e93a0-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
