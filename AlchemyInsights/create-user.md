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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747026"
---
# <a name="create-user"></a>Vytvoriť používateľa

**OZNÁMENIE**

- [Odmietanie podpory pri prihlasovaní na webové stránky od spoločnosti Google od 4. januára 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Otestujte, či vaše aplikácie môžu byť ovplyvnené podľa [pokynov spoločnosti Google](https://go.microsoft.com/fwlink/?linkid=2157323) o testovaní kompatibility.
- Pri prihlasovaní používateľov pomocou spotrebiteľských kont Google sa uistite, že používate systémové webové zobrazenie alebo systémový prehliadač. Ďalšie informácie nájdete v téme [problémy s prihlasovaním do aplikácií pomocou prehliadača Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Nemôžem vytvoriť nového používateľa v službe Azure AD Directory**

1. Uistite sa, že máte oprávnenie na vytvorenie nového štandardného používateľa. Nový štandardný používateľ môže vytvoriť iba globálny správca alebo rola správcu používateľa v službe Azure Active Directory (AD). Ak nie ste v niektorej z týchto rolí, požiadajte správcu, aby vás pridal do niektorej z týchto rolí alebo aby vám vytvoril nové používateľské konto.
1. Skontrolujte, či sa meno používateľa nachádza v doméne, ktorá je overená v službe Azure AD. Ak nemáte žiadne overené vlastné názvy domén v službe Azure AD, môžete použiť pôvodnú doménu Azure AD, ktorá končí reťazcom *. onmicrosoft.com.
1. Skontrolujte, či sa meno používateľa nachádza v doméne, ktorá nie je združená s Azúrovou REKLAMou z lokálnej reklamy. Používatelia nie je možné pridať do cloudu s názvami domén, ktoré sú externé ako lokálne.
1. Uistite sa, že žiadny iný používateľ ani kontakt už nemá meno používateľa, ktoré chcete priradiť novému používateľovi. Mená používateľov musia byť jedinečné v rámci služby Azure AD.
1. Pozrite si tému [roly Azure AD a správcovia](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) služby Azure AD.
1. Pozrite si [názvy domén](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) v službe Azure AD.
1. Skontrolujte [denníky auditu](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) , aby sa zobrazili podrobnejšie informácie o nedávno vytvorenom alebo odstránenom používateľovi, ako ktorí vykonali akciu, a kedy.
1. Ďalšie informácie o pridávaní nových používateľov nájdete [v téme Používanie portálu Azure na vytvorenie nového používateľa v službe Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Roly spravovania služby Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): povolenia roly správcu v službe Azure Active Directory
1. [Na vytvorenie nového používateľa môžete použiť aj prostredie Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
