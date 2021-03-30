---
title: Single-Sign v zariadeniach pripojených k službe Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405660"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="029e3-102">Jediné prihlásenie pre pripojené zariadenia Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="029e3-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="029e3-103">Ak máte lokálne prostredie služby Active Directory (AD) a chcete sa pripojiť k počítačom pripojeným k doméne AD do služby Azure AD, môžete to dosiahnuť hybridným spojením so službou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="029e3-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="029e3-104">[Postup: Plánovanie hybridnej implementácie](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) spojenia so službou Azure Active Directory vám poskytuje súvisiace kroky na implementáciu hybridného spojenia so službou Azure AD vo vašom prostredí.</span><span class="sxs-lookup"><span data-stu-id="029e3-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="029e3-105">Konfigurácia pripojených zariadení so službou Azure AD pre lokálne Single-Sign pomocou funkcie Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="029e3-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="029e3-106">**Problémy s primárnym obnovovacím tokenom (PRT)** Primárny obnovovací token (PRT) je kľúčovou artefaktou overovania Azure AD vo Windowse 10, Windows Serveri 2016 a novších verziách, zariadeniach so systémom iOS a Android.</span><span class="sxs-lookup"><span data-stu-id="029e3-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="029e3-107">Je to JSON Web Token (JWT) špeciálne vydaný sprostredkovateľom tokenov prvej strany spoločnosti Microsoft, ktorý umožňuje jediné prihlásenie (SSO) v aplikáciách používaných v týchto zariadeniach.</span><span class="sxs-lookup"><span data-stu-id="029e3-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="029e3-108">[V časti Čo je hlavný obnovovací token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)vám poskytneme podrobnosti o spôsobe vydania, používania a ochrany PRT v zariadeniach s Windowsom 10.</span><span class="sxs-lookup"><span data-stu-id="029e3-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="029e3-109">**WamDefaultSet: YES a AzureADPrt: YES** Tieto polia označujú, či sa používateľ úspešne overil v službe Azure AD pri prihlasovaní do zariadenia.</span><span class="sxs-lookup"><span data-stu-id="029e3-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="029e3-110">Ak hodnoty nie sú **,** môže to byť spôsobené:</span><span class="sxs-lookup"><span data-stu-id="029e3-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="029e3-111">Bad storage key in the TPM associated with the device upon registration (kontrola KeySignTest pri spustení zvýšených).</span><span class="sxs-lookup"><span data-stu-id="029e3-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="029e3-112">Alternatívne prihlasovacie ID</span><span class="sxs-lookup"><span data-stu-id="029e3-112">Alternate Login ID</span></span>
- <span data-ttu-id="029e3-113">Server HTTP Proxy sa nenašiel</span><span class="sxs-lookup"><span data-stu-id="029e3-113">HTTP Proxy not found</span></span>

<span data-ttu-id="029e3-114">Riešenie problémov so zariadeniami pomocou príkazu dsregcmd – [stav jediného prihlásenia](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="029e3-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
