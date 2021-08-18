---
title: Vytvoriť používateľa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323301"
---
# <a name="create-user"></a>Vytvoriť používateľa

**OZNÁMENIE:**

- [Od 4. januára 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) sme podporu pri prihlasovaní do služby WebView od spoločnosti Google odstrašujú. Pomocou pokynov spoločnosti Google o testovaní [kompatibility môžete testovať,](https://go.microsoft.com/fwlink/?linkid=2157323) či môžu byť vaše aplikácie ovplyvnené.
- Pri prihlasovaní používateľov pomocou spotrebiteľských kont Google nezabudnite používať systémové webové zobrazenie alebo systémový prehliadač. Ďalšie informácie nájdete v téme [Problémy pri prihlasovaní do aplikácií len pomocou prehliadača Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Nemôžem vytvoriť nového používateľa v adresári Azure AD**

1. Uistite sa, že máte oprávnenie na vytvorenie nového štandardného používateľa. Nového štandardného používateľa môže vytvoriť iba rola globálneho Azure Active Directory správcu alebo správcu používateľov v službe Azure Active Directory (AD). Ak nemáte niektorú z týchto rolí, požiadajte správcu, aby vás k jednej z týchto rolí pridať, alebo aby pre vás vytvoril nové používateľské konto.
1. Overte, či sa meno používateľa nachádza v doméne overenej v službe Azure AD. Ak nemáte v Azure AD žiadne overené vlastné názvy domén, môžete použiť počiatočnú doménu služby Azure AD, ktorá sa končí na *.onmicrosoft.com.
1. Skontrolujte, či sa meno používateľa nachádza v doméne, ktorá nie je federovaná na Azure AD z lokálnej služby AD. Používateľov nie je možné pridať do cloudu s názvami domén, ktoré sú federované z lokálneho objektu.
1. Presvedčte sa, že žiaden iný používateľ alebo kontakt už nemá meno používateľa, ktoré chcete priradiť novému používateľovi. V Azure AD musia byť mená používateľov jedinečné.
1. Pozrite [si roly a správcov služby Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pre službu Azure AD.
1. Pozrite si [názvy domén v](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
1. Pozrite [si denníky](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) auditu a pozrite si podrobnejšie informácie o nedávno vytvorenom alebo odstránenom používateľovi, napríklad kto a kedy akciu vykonal.
1. Ďalšie informácie o pridávaní nových používateľov nájdete v téme Vytvorenie nového používateľa v službe Azure AD pomocou [portálu Azure.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Roly správcu služby Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)povolenia roly správcu v Azure Active Directory
1. Na vytvorenie nového používateľa môžete použiť aj [Azure AD PowerShell.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
