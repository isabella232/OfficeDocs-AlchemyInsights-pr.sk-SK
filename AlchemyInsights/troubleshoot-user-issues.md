---
title: Riešenie problémov používateľov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901337"
---
# <a name="announcements"></a>Oznámenia

Postupujte podľa pokynov spoločnosti Google o testovaní kompatibility a otestujte, či sú vaše aplikácie ovplyvnené. Usmernenie spoločnosti Google je k dispozícii v programe https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Pri prihlasovaní používateľov pomocou spotrebiteľských kont Google sa uistite, že používate systémové webové zobrazenie alebo systémový prehliadač. Ďalšie informácie nájdete v téme [problémy s prihlasovaním do aplikácií pomocou prehliadača Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Nemôžem vytvoriť nového používateľa v službe Azure AD Directory**

Ak chcete vyriešiť problém, že nie je možné vytvoriť nového používateľa v službe Azure AD, vykonajte tieto kroky:

1. Uistite sa, že máte oprávnenie na vytvorenie nového štandardného používateľa. Nový štandardný používateľ môže vytvoriť iba globálny správca alebo rola správcu používateľa v službe Azure Active Directory (AD). Ak nie ste v niektorej z týchto rolí, požiadajte správcu, aby vás pridal do niektorej z týchto rolí alebo aby vám vytvoril nové používateľské konto.
2. Skontrolujte, či sa meno používateľa nachádza v doméne, ktorá je overená v službe Azure AD. Ak nemáte žiadne overené vlastné názvy domén v službe Azure AD, môžete použiť pôvodnú doménu Azure AD, ktorá končí reťazcom *. onmicrosoft.com.
3. Skontrolujte, či sa meno používateľa nachádza v doméne, ktorá nie je združená s Azúrovou REKLAMou z lokálnej reklamy. Používatelia nie je možné pridať do cloudu s názvami domén, ktoré sú externé ako lokálne.
4. Uistite sa, že žiadny iný používateľ ani kontakt už nemá meno používateľa, ktoré chcete priradiť novému používateľovi. Mená používateľov musia byť jedinečné v rámci služby Azure AD.
5. Pozrite si tému [roly Azure AD a správcovia](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) služby Azure AD.
6. Pozrite si [názvy domén](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) v službe Azure AD.
7. Skontrolujte [denníky auditu](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) , aby sa zobrazili podrobnejšie informácie o nedávno vytvorenom alebo odstránenom používateľovi, ako ktorí vykonali akciu, a kedy.
8. Ďalšie informácie o pridávaní nových používateľov nájdete [v téme Používanie portálu Azure na vytvorenie nového používateľa v službe Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Ďalšie informácie o povoleniach roly správcu v službe Azure AD nájdete v téme [roly spravovania služby Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Podrobnosti o vytváraní používateľa pomocou prostredia Azure AD PowerShell nájdete v téme [Azure AD PowerShell na vytvorenie nového používateľa](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problém so zaregistrovaním vlastnej služby**

Ak chcete riešiť problémy týkajúce sa registrácie vlastnej služby, vykonajte tieto kroky:

1. Ak chcete používať registráciu s vlastným servisom s vašimi aplikáciami, najprv povoľte registráciu pre nájomníka. 
2. Ak chcete povoliť aplikáciu, ktorá podporuje registráciu vlastnej služby, pridajte ju do svojho používateľského toku. Pri ďalšom prechode na prihlasovaciu stránku pre danú aplikáciu sa zobrazí možnosť **_žiadne konto? Vytvorte si ho._* _. Spustí sa proces registrácie samoobslužné.
3. Informácie o tom, ako používať samoobslužné Zaregistrujte sa na vyplnenie organizácie v službe Azure AD, nájdete v téme [Automatická registrácia v službe Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Po priradení toku používateľa k jednej alebo viacerým aplikáciám budú môcť používatelia, ktorí navštívia túto aplikáciu, zaregistrovať a získať hosťovské konto pomocou možností konfigurovaných v toku používateľa. Ak chcete získať ďalšie informácie o registrácii a získaní hosťovského konta, používatelia môžu v [prípade hosťujúcich používateľov zobraziť samoobslužné prihlásenie](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problém s pozvaním externého používateľa**

Ak chcete riešiť problémy týkajúce sa pozvania externého používateľa, vykonajte nasledujúci krok:

Uistite sa, že odošlete pozvánku používateľa na e-mailovú adresu, ktorá sa zhoduje s menom, ku ktorému sa používateľ prihlási. Ak odošlete pozvánku na e-mailovú adresu proxy používateľa, používateľ ju nemôže uplatniť. Ďalšie informácie nájdete v téme [Azure AD B2B dokumentáciu](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Nemôžem priradiť licencie používateľovi**

Ak chcete riešiť problémy týkajúce sa priraďovania licencií používateľovi, vykonajte tieto kroky:

1. Ak chcete spravovať používateľské licencie, uistite sa, že používate konto s niektorou z požadovaných rolí správcu: globálnym správcom, správcom licencií alebo správcom používateľa. Rolu používateľa môžete skontrolovať na karte **rola adresára** na používateľskom Blade.
2. Ak používate Azure Portal a priradenie licencie zlyháva, kliknite na oznámenie v pravom hornom rohu. Tým sa otvorí čepeľ s podrobnosťami o tom, čo sa stalo. Vo väčšine prípadov stačí porozumieť a vyriešiť problém.
3. Pred priradením licencie používateľovi sa uistite, že vlastnosť **umiestnenia využitia** je nastavená pre používateľa. Overte, či má používateľ túto vlastnosť nastavenú zobrazením karty **profil** na používateľskom Blade.
4. Uistite sa, že je k dispozícii dostatok licencií na produkt, ktorý sa pokúšate priradiť. Počet dostupných licencií môžete zobraziť na portáli Azure v službe [Azure Active Directory – licencie na > – > všetky produkty](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Používateľ už môže mať inú licenciu, ktorej služby sú v rozpore s tými, ktoré sú v novej licencii, ktorú sa pokúšate priradiť. Ak má napríklad používateľ zapnutú službu Exchange Online (plán 1), nebudete môcť priradiť licenciu k službe Exchange Online (Plan 2). Zakážte jednu zo služieb, aby sa povolila nová priradená licencia. Ak používate Azure Portal alebo rutiny typu cmdlet prostredia PowerShell, stránka s **podrobnosťami o probléme** obsahuje konkrétne služby, ktoré spôsobujú konflikt.
6. Ak sa pokúšate odobrať licenciu a ktorá zlyháva, používateľ môže mať iné licencie so službami, ktoré závisia od služieb, ktoré sa pokúšate odstrániť. Ak používate Azure Portal alebo rutiny typu cmdlet prostredia PowerShell, v chybovom hlásení sa zobrazí zoznam konkrétnych služieb, ktoré majú závislosti.
7. Ak chcete pochopiť, prečo bola licencia priradená alebo odstránená od používateľa (napríklad kto iný vo vašej organizácii vykonal zmeny), skontrolujte denníky auditu. Nastavte filter na **licenčné aktivity** , aby sa zobrazili všetky zmeny vrátane herca, ktorý ich vykonal.
8. Ak používate Exchange Online, niektorých používateľov v nájomníkovi môže byť nesprávne nakonfigurované s tou istou adresou proxy. V takýchto prípadoch sa pri zlyhaní licenčnej operácie môžu zobraziť všeobecné chybové hlásenia. [Tento článok](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) obsahuje ďalšie informácie o tomto probléme vrátane informácií o [tom, ako sa pripojiť k službe Exchange Online pomocou vzdialeného prostredia PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Ak chcete zistiť, ktorí používatelia v nájomníkovi obsahujú rovnakú adresu servera proxy, spustite túto rutinu typu cmdlet služby Exchange Online:

Spustiť

Get-Recipient | kde {$ _. EmailAddresss-Match <user principal name> } | fL Name, RecipientType nastavená, emailaddresss





