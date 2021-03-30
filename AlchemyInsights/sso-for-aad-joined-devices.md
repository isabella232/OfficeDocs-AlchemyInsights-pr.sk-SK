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
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Jediné prihlásenie pre pripojené zariadenia Azure Active Directory

Ak máte lokálne prostredie služby Active Directory (AD) a chcete sa pripojiť k počítačom pripojeným k doméne AD do služby Azure AD, môžete to dosiahnuť hybridným spojením so službou Azure AD. [Postup: Plánovanie hybridnej implementácie](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) spojenia so službou Azure Active Directory vám poskytuje súvisiace kroky na implementáciu hybridného spojenia so službou Azure AD vo vašom prostredí.

[Konfigurácia pripojených zariadení so službou Azure AD pre lokálne Single-Sign pomocou funkcie Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problémy s primárnym obnovovacím tokenom (PRT)** Primárny obnovovací token (PRT) je kľúčovou artefaktou overovania Azure AD vo Windowse 10, Windows Serveri 2016 a novších verziách, zariadeniach so systémom iOS a Android. Je to JSON Web Token (JWT) špeciálne vydaný sprostredkovateľom tokenov prvej strany spoločnosti Microsoft, ktorý umožňuje jediné prihlásenie (SSO) v aplikáciách používaných v týchto zariadeniach. [V časti Čo je hlavný obnovovací token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)vám poskytneme podrobnosti o spôsobe vydania, používania a ochrany PRT v zariadeniach s Windowsom 10.

**WamDefaultSet: YES a AzureADPrt: YES** Tieto polia označujú, či sa používateľ úspešne overil v službe Azure AD pri prihlasovaní do zariadenia. Ak hodnoty nie sú **,** môže to byť spôsobené:

- Bad storage key in the TPM associated with the device upon registration (kontrola KeySignTest pri spustení zvýšených).
- Alternatívne prihlasovacie ID
- Server HTTP Proxy sa nenašiel

Riešenie problémov so zariadeniami pomocou príkazu dsregcmd – [stav jediného prihlásenia](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
