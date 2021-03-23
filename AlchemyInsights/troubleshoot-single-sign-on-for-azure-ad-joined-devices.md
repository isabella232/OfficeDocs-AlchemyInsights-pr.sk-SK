---
title: Riešenie problémov s jediným prihlásením k zariadeniam pripojeného k službe Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037332"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="70260-102">Riešenie problémov s jediným prihlásením k zariadeniam pripojeného k službe Azure AD</span><span class="sxs-lookup"><span data-stu-id="70260-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="70260-103">Ak máte prostredie služby Active Directory (AD) v lokálnom prostredí a chcete sa do počítača s doménou ad pridať k službe Azure AD, môžete to urobiť pomocou pripojenia hybridnej služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70260-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="70260-104">[Ako na to: Naplánovanie pripojenia hybridnej služby Azure Active Directory k implementácii](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vám poskytuje súvisiace kroky na implementáciu hybridného spojenia Azure AD vo vašom prostredí.</span><span class="sxs-lookup"><span data-stu-id="70260-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="70260-105">Ďalšie informácie nájdete v téme [Konfigurácia zariadení s pripojením Azure AD pre lokálne Single-Sign o používaní Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="70260-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="70260-106">**Hlavné problémy s tokenom obnovenia (PRT)**</span><span class="sxs-lookup"><span data-stu-id="70260-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="70260-107">Hlavným tokenom obnovenia (PRT) je kľúčový artefakt overovania Azure AD v zariadeniach s Windowsom 10, Windows Server 2016 a novších verziách, iOS a Android.</span><span class="sxs-lookup"><span data-stu-id="70260-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="70260-108">Ide o webový token JSON (JWT), ktorý bol špeciálne vydaný pre brokerov tokenov prvej strany spoločnosti Microsoft na povolenie jediného prihlásenia (SSO) v rámci aplikácií používaných v týchto zariadeniach.</span><span class="sxs-lookup"><span data-stu-id="70260-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="70260-109">Podrobnosti o tom, ako sa PRT vydáva, používa a chráni v zariadeniach s Windowsom 10, nájdete v téme [čo je primárny token obnovenia?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="70260-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="70260-110">**WamDefaultSet: Áno a AzureADPrt: Áno**</span><span class="sxs-lookup"><span data-stu-id="70260-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="70260-111">Tieto polia označujú, či sa používateľ úspešne overil na Azúrovom AD pri prihlasovaní do zariadenia.</span><span class="sxs-lookup"><span data-stu-id="70260-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="70260-112">Ak hodnoty **nie** sú, môže to byť spôsobené:</span><span class="sxs-lookup"><span data-stu-id="70260-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="70260-113">Chybný kód ukladacieho priestoru v module TPM priradeného k zariadeniu pri registrácii (kontrola KeySignTest pri spustení zvýšené)</span><span class="sxs-lookup"><span data-stu-id="70260-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="70260-114">Alternatívna identifikácia prihlásenia</span><span class="sxs-lookup"><span data-stu-id="70260-114">Alternate Login ID</span></span>
- <span data-ttu-id="70260-115">HTTP proxy sa nenašiel</span><span class="sxs-lookup"><span data-stu-id="70260-115">HTTP Proxy not found</span></span>

<span data-ttu-id="70260-116">Ak chcete riešiť problémy so zariadeniami pomocou príkazu dsregcmd, pozrite si tému [stav SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="70260-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
