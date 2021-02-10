---
title: Synchronizácia hash hesla pre službu Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177622"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="0eddf-102">Synchronizácia hash hesla pre službu Domain</span><span class="sxs-lookup"><span data-stu-id="0eddf-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="0eddf-103">**Ak sa na inštanciu služby Azure AD DS zobrazí výzva na povolenie synchronizácie hash hesla**</span><span class="sxs-lookup"><span data-stu-id="0eddf-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="0eddf-104">Narazíte na scenár, v ktorom používate hybridné prostredie s používateľmi, ktorí synchronizujú z lokálneho prostredia služby Azure Active Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="0eddf-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="0eddf-105">Tento scenár sa vyskytuje napriek tomu, že sa Synchronizácia hash hesla z lokálneho AD DS na nájomníka služby Azure AD nachádza.</span><span class="sxs-lookup"><span data-stu-id="0eddf-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="0eddf-106">**Príčina**</span><span class="sxs-lookup"><span data-stu-id="0eddf-106">**Cause**</span></span>

<span data-ttu-id="0eddf-107">To sa deje, pretože Azure AD Connect predvolene nesynchronizuje staršie nové technológie LAN Manager (NTLM) a Kerberos Password hash, ktoré sú potrebné pre Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="0eddf-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="0eddf-108">**Alternatívne riešenie**</span><span class="sxs-lookup"><span data-stu-id="0eddf-108">**Workaround**</span></span> 

<span data-ttu-id="0eddf-109">Ak chcete synchronizovať tieto hodnoty hash hesla vyžadované pre overovanie NTLM a Kerberos, budete musieť nakonfigurovať službu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="0eddf-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="0eddf-110">Po nakonfigurovaní služby Azure AD Connect sa pri vytvorení lokálneho konta alebo udalosti zmeny hesla potom synchronizuje staršie hash hesla k službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0eddf-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="0eddf-111">Ďalšie informácie o tejto téme a pokyny na Zapnutie synchronizácie hesiel v hybridných prostrediach Azure AD DS nájdete [tu](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) .</span><span class="sxs-lookup"><span data-stu-id="0eddf-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>