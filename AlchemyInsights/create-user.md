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
ms.openlocfilehash: afba00ffc6ba082606e0071b41e2917b11e6a39d61cd0df7e468f0238f2ed8e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118759"
---
# <a name="create-user"></a>Vytvoriť používateľa

**OZNÁMENIE:**

- [Od 4. januára 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) sme podporu pri prihlasovaní do služby WebView od spoločnosti Google odstrašujú. Pomocou pokynov spoločnosti Google o testovaní [kompatibility môžete testovať,](https://go.microsoft.com/fwlink/?linkid=2157323) či môžu byť vaše aplikácie ovplyvnené.
- Pri prihlasovaní používateľov pomocou spotrebiteľských kont Google nezabudnite používať systémové webové zobrazenie alebo systémový prehliadač. Ďalšie informácie nájdete v téme [Problémy pri prihlasovaní do aplikácií len pomocou prehliadača Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Nemôžem vytvoriť nového používateľa v adresári Azure AD**

1. Uistite sa, že máte oprávnenie na vytvorenie nového štandardného používateľa. Nového štandardného používateľa môže vytvoriť iba rola globálneho Azure Active Directory správcu alebo správcu používateľov v službe Azure Active Directory (AD). Ak nemáte niektorú z týchto rolí, požiadajte správcu, aby vás k jednej z týchto rolí pridať, alebo aby pre vás vytvoril nové používateľské konto.
1. Overte, či sa meno používateľa nachádza v doméne overenej v službe Azure AD. Ak nemáte v Azure AD žiadne overené vlastné názvy domén, môžete použiť počiatočnú doménu služby Azure AD, ktorá sa končí na *.onmicrosoft.com.
1. Skontrolujte, či sa meno používateľa nachádza v doméne, ktorá nie je federovaná na Azure AD z lokálnej služby AD. Používateľov nie je možné pridať do cloudu s názvami domén, ktoré sú federované z lokálneho objektu.
1. Presvedčte sa, že žiaden iný používateľ alebo kontakt už nemá meno používateľa, ktoré chcete priradiť novému používateľovi. V Azure AD musia byť mená používateľov jedinečné.
1. Pozrite [si časť Roly a správcovia služby Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pre službu Azure AD.
1. Pozrite si [názvy domén v](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
1. Pozrite [si denníky](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) auditu a pozrite si podrobnejšie informácie o nedávno vytvorenom alebo odstránenom používateľovi, napríklad kto a kedy akciu vykonal.
1. Ďalšie informácie o pridávaní nových používateľov nájdete v téme Vytvorenie nového používateľa v službe Azure AD pomocou [portálu Azure.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Roly správcu služby Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)povolenia roly správcu v Azure Active Directory
1. Na vytvorenie nového používateľa môžete použiť aj [Azure AD PowerShell.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
