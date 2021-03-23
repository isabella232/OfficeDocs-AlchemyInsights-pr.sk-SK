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
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Riešenie problémov s jediným prihlásením k zariadeniam pripojeného k službe Azure AD

Ak máte prostredie služby Active Directory (AD) v lokálnom prostredí a chcete sa do počítača s doménou ad pridať k službe Azure AD, môžete to urobiť pomocou pripojenia hybridnej služby Azure AD. [Ako na to: Naplánovanie pripojenia hybridnej služby Azure Active Directory k implementácii](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vám poskytuje súvisiace kroky na implementáciu hybridného spojenia Azure AD vo vašom prostredí.

Ďalšie informácie nájdete v téme [Konfigurácia zariadení s pripojením Azure AD pre lokálne Single-Sign o používaní Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Hlavné problémy s tokenom obnovenia (PRT)**

Hlavným tokenom obnovenia (PRT) je kľúčový artefakt overovania Azure AD v zariadeniach s Windowsom 10, Windows Server 2016 a novších verziách, iOS a Android. Ide o webový token JSON (JWT), ktorý bol špeciálne vydaný pre brokerov tokenov prvej strany spoločnosti Microsoft na povolenie jediného prihlásenia (SSO) v rámci aplikácií používaných v týchto zariadeniach. Podrobnosti o tom, ako sa PRT vydáva, používa a chráni v zariadeniach s Windowsom 10, nájdete v téme [čo je primárny token obnovenia?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: Áno a AzureADPrt: Áno**

Tieto polia označujú, či sa používateľ úspešne overil na Azúrovom AD pri prihlasovaní do zariadenia. Ak hodnoty **nie** sú, môže to byť spôsobené:

- Chybný kód ukladacieho priestoru v module TPM priradeného k zariadeniu pri registrácii (kontrola KeySignTest pri spustení zvýšené)
- Alternatívna identifikácia prihlásenia
- HTTP proxy sa nenašiel

Ak chcete riešiť problémy so zariadeniami pomocou príkazu dsregcmd, pozrite si tému [stav SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
