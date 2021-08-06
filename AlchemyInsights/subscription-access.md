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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999255"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nie je možné prihlásiť sa do služby Azure z dôvodu problémov v prehliadači (prehliadač sa zablokuje, stále otáča, nenačíta sa atď.)

Na vás môže mať vplyv výpadky. Skontrolujte, či prebieha prebiehajúci výpadku: [Stav služby Azure.](https://status.azure.com/status/history/)

Odhláste sa zo všetkých aktívnych relácií služby Azure. Spustite súkromný režim alebo režim inkognito webového prehliadača.

Môžete sa tiež pokúsiť obnoviť prehliadač, použiť iný prehliadač a odstrániť súbory cookie vyrovnávacej pamäte, ak vyššie uvedené nefunguje.

Ďalšie informácie: [Riešenie problémov s prihlásením](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nie je možné získať prístup k predplatným**

Na [portáli Azure](https://portal.azure.com/)skontrolujte, či je v konte v pravom hornom rohu vybratý správny adresár Azure.

V Centre [kont Azure skontrolujte,](https://account.windowsazure.com/Subscriptions)či je použité konto správcom konta.

Ďalšie informácie: Riešenie [problémov so žiadnymi predplatným](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nie je možné získať prístup k histórii fakturácie**

Správca konta musí zabezpečiť, aby sa používateľ, ktorý má prístup k fakturačným údajom, pridal do adresára Azure Active ako hosť: Pridanie alebo odstránenie [nového používateľa.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Používateľovi je potom potrebné priradiť rolu globálneho správcu: Priradiť [rolu používateľom.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Po tomto príspevku môže používateľ získať prístup k fakturácii pomocou politík pre politiku prístupu na základe prístupu na základe prístupu: [udelenie prístupu k fakturácii.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Odporučené dokumenty**

-   [Nemôžem sa prihlásiť na spravovanie svojho predplatného služby Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)