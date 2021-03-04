---
title: Problém s jediným používateľom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430206"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="8d088-102">Problém s jediným používateľom</span><span class="sxs-lookup"><span data-stu-id="8d088-102">Problem with single user</span></span>

- <span data-ttu-id="8d088-103">Používateľ nemusí byť zriadený, pretože služba ešte nemá možnosť hodnotenia používateľa.</span><span class="sxs-lookup"><span data-stu-id="8d088-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="8d088-104">Pozrite si usmernenie o tom, ako dlho bude poskytovanie trvať, ako aj indikátor priebehu na stránke konfigurácie poskytovania.</span><span class="sxs-lookup"><span data-stu-id="8d088-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="8d088-105">Ak je rovnovážny stav zadaný v časti Ďalšie podrobnosti pred dátumom vytvorenia/aktualizácie alebo odstránenia používateľa, znamená to, že sme zatiaľ nehodnotili používateľa.</span><span class="sxs-lookup"><span data-stu-id="8d088-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="8d088-106">V tomto scenári je najvhodnejšie počkať na dokončenie poskytovania služby.</span><span class="sxs-lookup"><span data-stu-id="8d088-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="8d088-107">Všimnite si, že naša služba je oboznámená len s zmenami používateľa v zdrojovom systéme (cloud HR).</span><span class="sxs-lookup"><span data-stu-id="8d088-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="8d088-108">Pri zisťovaní zmeny a jeho toku do služby Active Directory musí byť platná zmena v zdrojovom systéme pre Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d088-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="8d088-109">Poskytovanie služby vyhodnotilo používateľa a určilo sa, že by sa nemalo poskytovať:</span><span class="sxs-lookup"><span data-stu-id="8d088-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="8d088-110">Ak ste nastavili filter založený na atribútoch, overte, či používateľ spĺňa kritériá, ktoré ste zadali.</span><span class="sxs-lookup"><span data-stu-id="8d088-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="8d088-111">Ak už používatelia existujú v cieľovom systéme a stave používateľa v zdrojovej a cieľovej zhode, nebudeme mať žiadne ďalšie kroky.</span><span class="sxs-lookup"><span data-stu-id="8d088-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="8d088-112">Poskytovanie služby sa pokúsilo o poskytnutie používateľa a zlyhalo.</span><span class="sxs-lookup"><span data-stu-id="8d088-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="8d088-113">V prípade týchto scenárov si pozrite kartu Riešenie problémov a odporúčaní v denníkoch poskytovania:</span><span class="sxs-lookup"><span data-stu-id="8d088-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="8d088-114">V lokálnej službe Active Directory alebo službe Azure AD môže chýbať požadovaný atribút používateľa.</span><span class="sxs-lookup"><span data-stu-id="8d088-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="8d088-115">Pravidlá tvorby userPrincipalName alebo sAMAccountName napríklad nevytvárajú správnu hodnotu.</span><span class="sxs-lookup"><span data-stu-id="8d088-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="8d088-116">Zodpovedajúci atribút (zvyčajne klíč) sa nerieši jedinečnému používateľovi v lokálnej službe Active Directory alebo v službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d088-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="8d088-117">Napríklad existujú dvaja používatelia s rovnakým klíč v REKLAMe a služba vráti kód chyby označujúci duplicitné cieľové položky pre tú istú zdrojovú položku.</span><span class="sxs-lookup"><span data-stu-id="8d088-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="8d088-118">Ak chcete skontrolovať denníky pre jedného používateľa a skupiny, pozrite si tému [Revízia denníkov poskytovania problému s konkrétnym používateľom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="8d088-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
