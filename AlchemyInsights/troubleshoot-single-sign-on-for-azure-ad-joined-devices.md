---
title: Riešenie problémov s jediným prihlásením v zariadeniach pripojených k službe Azure AD
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
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039261"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Riešenie problémov s jediným prihlásením v zariadeniach pripojených k službe Azure AD

Ak máte lokálne prostredie služby Active Directory (AD) a chcete sa pripojiť k počítačom pripojeným k doméne AD do služby Azure AD, môžete to dosiahnuť hybridným spojením so službou Azure AD. [Postup: Plánovanie hybridnej implementácie Azure Active Directory pripojenie](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vám poskytuje súvisiace kroky na implementáciu hybridného spojenia so službou Azure AD vo vašom prostredí.

Ďalšie informácie nájdete v téme Konfigurácia pripojených zariadení so službou [Azure AD pre lokálne Single-Sign v Windows Hello for Business.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Problémy s primárnym obnovovacím tokenom (PRT)**

Primárny obnovovací token (PRT) je kľúčovou artefaktou overovania Azure AD v zariadeniach Windows 10, Windows Server 2016 a novších verziách, iOS a Android. Je to JSON Web Token (JWT) špeciálne vydaný sprostredkovateľom tokenov prvej strany spoločnosti Microsoft, ktorý umožňuje jediné prihlásenie (SSO) v aplikáciách používaných v týchto zariadeniach. Podrobnosti o tom, ako sa vydáva, používa a chráni PRT v Windows 10 zariadeniach, nájdete v téme Čo je [hlavný obnovovací token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES a AzureADPrt: YES**

Tieto polia označujú, či sa používateľ úspešne overil v službe Azure AD pri prihlasovaní do zariadenia. Ak sú hodnoty **NIE,** môže to byť spôsobené:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)
- Alternatívne prihlasovacie ID
- Server HTTP Proxy sa nenašiel

Informácie o riešení problémov so zariadeniami pomocou príkazu dsregcmd nájdete v téme [Stav jediného prihlásenia](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
