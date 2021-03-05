---
title: Problém s filtrom atribútu a rozsahu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482921"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="ea29a-102">Problém s filtrom atribútu a rozsahu</span><span class="sxs-lookup"><span data-stu-id="ea29a-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="ea29a-103">**Problém s kolidujúcimi hodnotami hlavného mena používateľa**</span><span class="sxs-lookup"><span data-stu-id="ea29a-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="ea29a-104">Pracovný deň na poskytovanie AD User (pracovný deň) na poskytovanie AD používateľov zobrazuje chybové hlásenie **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="ea29a-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="ea29a-105">Operácia zlyhala, pretože hodnota hlavného mena používateľa poskytnutá na sčítanie alebo úpravu nie je jedinečná.</span><span class="sxs-lookup"><span data-stu-id="ea29a-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="ea29a-106">Podrobnosti o chybe: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="ea29a-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="ea29a-107">Hodnota **userPrincipalName** , ktorá sa pri vytváraní používateľského konta v reklame, ktorá sa pokúša nastaviť, sa v doméne cieľová reklama už vyskytuje.</span><span class="sxs-lookup"><span data-stu-id="ea29a-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="ea29a-108">To znamená, že buď (1) používateľ už existuje, a kontrola zhodných IDENTIFIKÁCIí pre používateľa zlyhala alebo (2) pravidlo generácie UPN vygenerovalo kolidujúcu hodnotu.</span><span class="sxs-lookup"><span data-stu-id="ea29a-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="ea29a-109">Tu sú navrhované kroky riešenia:</span><span class="sxs-lookup"><span data-stu-id="ea29a-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="ea29a-110">Ak už používateľ existuje a kontrola TOTOŽNosti sa nepodarilo prepojiť konto pracovného dňa s kontom služby Active Directory, skontrolujte, či sa zhoda s atribútom ID (zvyčajne **klíč**) v oboch pracovný deň aj v reklame presne zhoduje.</span><span class="sxs-lookup"><span data-stu-id="ea29a-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="ea29a-111">Ak sa nezhodujú, ide o problém s údajmi, ktorý treba opraviť.</span><span class="sxs-lookup"><span data-stu-id="ea29a-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="ea29a-112">Ak je napríklad identifikácia zamestnanca v pracovnom hárku 001052 a v REKLAMe je 1052, potom sa pri zriaďovaní motora nepodarí prepojiť dva kontá a pokúsiť sa vytvoriť používateľa, ktorý už existuje.</span><span class="sxs-lookup"><span data-stu-id="ea29a-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="ea29a-113">Riešenie v tomto prípade je zmeniť hodnotu **klíč** v reklame tak, aby obsahovala úvodné nuly, aby bolo 001052.</span><span class="sxs-lookup"><span data-stu-id="ea29a-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="ea29a-114">Ak výraz generovanie UPN nevytvára jedinečnú hodnotu, zvážte použitie funkcie de-duplikácie **SelectUniqueValue** na vytvorenie jedinečnej hodnoty pri každom spustení.</span><span class="sxs-lookup"><span data-stu-id="ea29a-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="ea29a-115">**Pracovný deň na poskytovanie AD User nenastaví hodnotu atribútu Manager pre konto AD User**</span><span class="sxs-lookup"><span data-stu-id="ea29a-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="ea29a-116">V pracovnom postupe AD User na poskytovanie úloh sa nenastaví hodnota atribútu **Manager** pre kontá ad user.</span><span class="sxs-lookup"><span data-stu-id="ea29a-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="ea29a-117">Ak sa toto správanie zobrazuje, existujú dva možné scenáre:</span><span class="sxs-lookup"><span data-stu-id="ea29a-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="ea29a-118">Manažér v pracovný deň nie je možné preložiť na zodpovedajúce konto AD User, pretože manažér nie je v rozsahu.</span><span class="sxs-lookup"><span data-stu-id="ea29a-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="ea29a-119">V scenári s **viacerými reklamnými doménami** sa manažér v pracovný deň nenachádza v rovnakej doméne ako používateľ.</span><span class="sxs-lookup"><span data-stu-id="ea29a-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="ea29a-120">Skúste problém vyriešiť pomocou týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="ea29a-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="ea29a-121">Ak ste definovali rozsahy filtrov, najskôr skontrolujte, či je manažér v rozsahu a či spĺňa klauzulu rozsahov.</span><span class="sxs-lookup"><span data-stu-id="ea29a-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="ea29a-122">Ak manažér nevyhovuje filtru rozsahu, zmeňte filter tak, aby bol manažér v rozsahu operácie poskytovania.</span><span class="sxs-lookup"><span data-stu-id="ea29a-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="ea29a-123">Ak máte viacero REKLAMných domén, konektor má známe obmedzenie nemožnosti riešenia odkazov na krížový správca domény.</span><span class="sxs-lookup"><span data-stu-id="ea29a-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="ea29a-124">Ďalšie informácie o konfigurácii pracovného dňa na automatické poskytovanie informácií nájdete v téme [kurz: Konfigurácia pracovného dňa na automatické poskytovanie používateľov](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="ea29a-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













