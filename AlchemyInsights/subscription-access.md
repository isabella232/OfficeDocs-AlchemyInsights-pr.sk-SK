---
title: Prístup k predplatnému
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807721"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Azure sa nedá prihlásiť v dôsledku problémov s prehliadačom (prehliadač sa zablokuje, udržuje spinning, nenačíta sa atď.)

Môže sa stať, že budete mať vplyv na výpadok. Skontrolujte, či sa vyskytol pokračujúci výpadok: [stav služby Azure Health](https://status.azure.com/status/history/).

Odhláste sa zo všetkých aktívnych relácií služby Azure. Spustite režim v súkromí alebo v režime inkognito webového prehliadača.

Môžete sa tiež pokúsiť obnoviť prehliadač, použiť iný prehliadač, odstrániť súbory cookie vyrovnávacej pamäte, ak vyššie uvedené nefunguje.

Ďalšie informácie: [Riešenie problémov s prihlasovaním](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nie je možné získať prístup k predplatnému**

Na [portáli Azure](https://portal.azure.com/)Skontrolujte, či je v pravom hornom rohu vybratá správna adresár Azure.

Skontrolujte, či je v [centre Azure Account](https://account.windowsazure.com/Subscriptions)(konto) konto správcu konta.

Ďalšie informácie: [Riešenie problémov s nenájdenými predplatnými](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nie je možné získať prístup k histórii fakturácie**

Správca konta potrebuje uistiť sa, že používateľ s prístupom k informáciám o fakturácii sa pridá do služby Azure Active Directory ako hosťovský používateľ: [Pridanie alebo odstránenie nového používateľa](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Používateľovi sa potom musí dostať rola globálneho správcu: [Priradenie roly používateľom](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Zverejniť tento príspevok môže mať používateľ prístup na fakturáciu pomocou politík RBAC: [udelenie prístupu k fakturácii](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Odporúčané dokumenty**

-   [Nemôžem sa prihlásiť na spravovanie môjho predplatného Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)