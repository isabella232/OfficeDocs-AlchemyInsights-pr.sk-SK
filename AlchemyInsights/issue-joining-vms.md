---
title: Problém s pripojením k VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885662"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="8d0ab-102">Problém s pripojením k VMs</span><span class="sxs-lookup"><span data-stu-id="8d0ab-102">Issue joining VMs</span></span>

<span data-ttu-id="8d0ab-103">Ak chcete vyriešiť problémy, ktoré sa vyskytujú pri pokuse o spojenie s VMs, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="8d0ab-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="8d0ab-104">Skúste sa prihlásiť pomocou formátu **UPN** (napríklad "JoeUser@contoso.com") namiesto formátu **SAMAccountName** (' CONTOSO\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="8d0ab-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="8d0ab-105">Skontrolujte, či ste povolili synchronizáciu hesiel v súlade s krokmi uvedenými v *príručke Začíname* .</span><span class="sxs-lookup"><span data-stu-id="8d0ab-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="8d0ab-106">Skontrolujte, či príslušné používateľské konto nie je externým kontom v nájomníkovi služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d0ab-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="8d0ab-107">Externí používatelia sa nemôžu prihlásiť do spravovanej domény, pretože služby Azure AD Domain neobsahujú poverenia pre takéto používateľské kontá.</span><span class="sxs-lookup"><span data-stu-id="8d0ab-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="8d0ab-108">Ak je postihnuté používateľské konto iba v cloude, zabezpečte, aby používatelia zmenili svoje heslo po zapnutí služby Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="8d0ab-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="8d0ab-109">Tento krok spôsobuje hodnoty hash poverení vyžadované na generovanie služieb Azure AD domain.</span><span class="sxs-lookup"><span data-stu-id="8d0ab-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="8d0ab-110">Ak sa príslušné používateľské kontá synchronizujú z lokálneho adresára, overte, či je odporúčaná verzia služby Azure AD Connect nakonfigurovaná na vykonanie úplnej synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="8d0ab-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="8d0ab-111">Ak problémy pretrvávajú aj po potvrdení kroku 4, spustite nasledujúce príkazy zo zariadenia na synchronizáciu:</span><span class="sxs-lookup"><span data-stu-id="8d0ab-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="8d0ab-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="8d0ab-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>