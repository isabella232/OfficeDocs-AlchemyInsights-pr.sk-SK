---
title: Riešenie chyby Aplikácia nebola rozpoznaná
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836366"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="09f1e-102">Riešenie chyby Aplikácia nebola rozpoznaná</span><span class="sxs-lookup"><span data-stu-id="09f1e-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="09f1e-103">Chyba inštalácie aplikácie „Aplikácia nebola rozpoznaná po úspešnom dokončení inštalácie“ nahlásená službou Intune sa môže vyskytnúť vo všetkých hlavných platformách operačného systému (Windows, iOS a Android).</span><span class="sxs-lookup"><span data-stu-id="09f1e-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="09f1e-104">Najbežnejšie scenáre, pri ktorých sa vyskytne táto chyba, zahŕňajú:</span><span class="sxs-lookup"><span data-stu-id="09f1e-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="09f1e-105">Aplikácia bola aktualizovaná mimo služby Intune (z obchodu s aplikáciami tretej strany) po počiatočnom nasadení.</span><span class="sxs-lookup"><span data-stu-id="09f1e-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="09f1e-106">Príklad: Niektoré aplikácie, napríklad Google Chrome, môžu vykonávať automatické aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="09f1e-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="09f1e-107">Používateľ odinštaloval aplikáciu po počiatočnej inštalácii.</span><span class="sxs-lookup"><span data-stu-id="09f1e-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="09f1e-108">Ak chcete vyriešiť tento problém, najskôr skontrolujte ovplyvnené zariadenia a zistite, v ktorom scenári sa chyba vyskytuje.</span><span class="sxs-lookup"><span data-stu-id="09f1e-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="09f1e-109">Ak bola aplikácia aktualizovaná mimo služby Intune, nasadenie aplikácie je možné nastaviť na ignorovanie verzie aplikácie.</span><span class="sxs-lookup"><span data-stu-id="09f1e-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="09f1e-110">Ak to chcete urobiť, v časti **Konfigurácia aplikácie > Informácie o aplikácii** nastavte položku **Ignorovaťnú verziu aplikácie** na možnosť **Áno**.</span><span class="sxs-lookup"><span data-stu-id="09f1e-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="09f1e-111">Pri zacielení na klienta môže byť vhodné nasadiť aplikáciu ako „povinnú“ a zabezpečiť, aby sa nasadila najnovšia verzia.</span><span class="sxs-lookup"><span data-stu-id="09f1e-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="09f1e-112">Prípadne na platforme iOS je možné použiť funkciu **automatickej aktualizácie** spojenej s programom Apple Volume Purchase Program, ktorú je možné nakonfigurovať tak, aby automaticky aktualizovala na nové verzie aplikácií, keď budú k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="09f1e-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="09f1e-113">Ďalšie informácie o riešení problémov s inštaláciou aplikácií nájdete v téme [Riešenie problémov s inštaláciou aplikácií](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="09f1e-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
