---
title: Priradenia atribútov zabezpečenia používateľa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949895"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="f30ab-102">Priradenia atribútov zabezpečenia používateľa</span><span class="sxs-lookup"><span data-stu-id="f30ab-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="f30ab-103">Ak chcete riešiť problémy so známym priradením atribútov, pozrite si tému [priradenia atribútov](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="f30ab-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="f30ab-104">Microsoft Azure Active Directory (AD) poskytuje podporu pre poskytovanie používateľov na aplikácie SaaS tretích strán, ako je napríklad Salesforce, G Suite a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="f30ab-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="f30ab-105">Ak zapnete poskytovanie používateľov pre aplikáciu SaaS tretej strany, na portáli Azure sa riadia hodnoty atribútov prostredníctvom priradení atribútov.</span><span class="sxs-lookup"><span data-stu-id="f30ab-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="f30ab-106">Informácie o prispôsobení predvolených priradení atribútov nájdete [v téme Prispôsobenie priradenia atribútov priradenia používateľov k aplikáciám SaaS v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="f30ab-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="f30ab-107">Ďalšie informácie o zriaďovaní používateľov služby SaaS nájdete v téme [čo je poskytovanie automatizovaných používateľských aplikácií SaaS v službe Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="f30ab-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="f30ab-108">Pri prispôsobovaní priradení atribútov pre poskytovanie používateľov sa môže stať, že sa atribút, ktorý chcete priradiť, nezobrazuje v zozname zdrojových atribútov.</span><span class="sxs-lookup"><span data-stu-id="f30ab-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="f30ab-109">[Synchronizácia atribútu z lokálnej služby Active Directory do služby Azure AD na poskytovanie](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) v článku aplikácie vám ukáže, ako pridať chýbajúci atribút tak, že ho synchronizujete z lokálnej reklamy na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f30ab-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
