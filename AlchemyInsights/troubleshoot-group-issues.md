---
title: Riešenie problémov skupiny
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714046"
---
# <a name="troubleshoot-group-issues"></a>Riešenie problémov skupiny

**Musím priradiť skupinu k úlohe Azure AD**

Ak chcete priradiť skupinu služby Azure Active Directory (AD) ku úlohe služby Azure AD, vykonajte tieto kroky:

1. Vytvorenie novej skupiny – vytvorenie novej skupiny:

    a. Prihláste sa do centra spravovania služby Azure AD s privilegovaným správcom roly alebo povoleniami globálneho správcu. 
    b. Vyberte položku Azure Active Directory > skupiny > všetky skupiny > novú skupinu. 
    c. Vytvorte skupinu.

2. Priraďte rolu skupine buď počas vytvárania skupiny alebo po vytvorení skupiny.

    a. Ak chcete skupine priradiť rolu v čase vytvárania skupiny, zapnite funkciu prepnutia funkcií Azure AD môže byť priradená skupine a vytvorte skupinu.
    b. Ak chcete priradiť rolu k skupine po jej vytvorení, prejdite na kartu priradené roly pre novo vytvorenú skupinu a priraďte rolu skupine.

**Potrebujem spravovať členstvo v skupine, ktorá je priradená k úlohe Azure AD**

1. Ak chcete zabrániť zvýšeniu počtu privilégií, na základe predvoleného nastavenia môže zmeniť členstvo skupiny, ktorá je priradená k úlohe, iba privilegovaný správca rolí a globálny správca. Môže sa však rozhodnúť priradiť vlastníkovi takejto skupiny a delegovať túto úlohu. Ďalšie informácie nájdete v téme [Používanie cloudových skupín na spravovanie priradení rolí v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Všeobecné otázky a tipy na riešenie problémov pri priraďovaní rolí skupinám v službe Azure AD nájdete v téme [Riešenie problémov priradených k cloudovým skupinám](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dynamické skupiny**

1. Ak nemôžete nájsť vstavané atribúty používateľa, skontrolujte, či sa atribút nachádza v zozname podporovaných vlastností.
2. Ak hľadáte vstavané atribúty zariadenia, zabezpečte, aby sa atribút nachádzal v zozname atribútov zariadenia 
3. Okrem vstavaných atribútov používateľa a zariadenia môžete použiť aj [atribúty prípony](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Po synchronizácii atribútov rozšírenia z lokálnej reklamy systému Windows Server alebo z pripojenej aplikácie SaaS by sa atribúty mali zobraziť v rozbaľovacom zozname Zostavovača pravidiel. Názov vlastnej atribútu sa nachádza v adresári dotazom na atribút používateľa pomocou prostredia PowerShell a vyhľadávaním názvu atribútu. Tieto pravidlá sa môžu použiť aj pri zostavovaní pravidiel v syntaxi pravidla.
4. Presvedčte sa, že váš nájomník má príslušnú licenciu. Dynamické skupiny vyžadujú, aby nájomník mal licenciu na Azure AD P1 Premium. K dispozícii je zoznam licenčných plánov Azure [ad.](https://azure.microsoft.com/pricing/details/active-directory/) K dispozícii sú tieto plány licencií Enterprise mobility + [Security.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Uistite sa, že úloha používateľa vytvárajúceho dynamickú skupinu je globálnym správcom, správcom služby Intune, správcom skupiny alebo správcom používateľa.
6. Počkajte, kým sa skupina zadá. V závislosti od veľkosti vášho nájomníka môže skupina trvať až 24 hodín, kým sa prvý raz doplní alebo sa zmení pravidlo.
7. Ďalšie informácie nájdete v téme [Vytvorenie pravidiel založených na atribútoch pre dynamické členstvo v skupine](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Potrebujem odstrániť skupinu**

1. Skupiny možno z adresára odstrániť pomocou rutiny typu cmdlet Remove-AzureADGroup v module Azure AD PowerShell.
2. Pred pokusom o odstránenie synchronizovanej skupiny v službe Azure AD sa uistite, že ste odstránili všetky priradené licencie, aby sa predišlo chybám.
3. Ďalšie informácie o odstraňovaní skupín nájdete v téme [Odstránenie skupiny s priradenou licenciou](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Musím obnoviť odstránenú skupinu**

1. Ak je skupina služieb Office 365 odstránená, môže sa obnoviť až 30 dní pred trvalým odstránením. Po trvalom odstránení sa skupina už nedá obnoviť. Ďalšie informácie o obnove skupín [nájdete tu](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Táto funkcia nie je podporovaná pre skupiny zabezpečenia a distribučné skupiny.
3. Uistite sa, že máte oprávnenie na obnovenie skupiny v Office 365. Globálni správcovia, Správcovia skupiny, správcovia používateľských kont, správcovia služieb služby Intune, partneri Tier1 alebo Tier2 support a vlastník skupiny môže byť schopný obnoviť skupinu.
4. Po odstránení a obnovení dynamickej skupiny sa táto skupina zobrazí ako nová skupina a znova sa vyplní podľa pravidla. Tento proces môže trvať až 24 hodín.
5. Ďalšie informácie o obnovení odstránenej skupiny nájdete [v téme Obnovenie odstránenej skupiny v Office 365 v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Konfigurácia politiky uplynutia platnosti skupiny**

1. Táto funkcia je podporovaná len pre skupiny v Office 365, nie však pre skupiny zabezpečenia a distribučné skupiny, nie sú podporované.
2. Konfigurácia a používanie politiky uplynutia platnosti pre skupiny v Office 365 vyžaduje licenciu Azure AD Premium.
3. V súčasnosti je možné nakonfigurovať iba jednu politiku uplynutia platnosti pre skupiny v Office 365 v nájomníkovi.
4. Skupinu môžu obnoviť len globálni správcovia, Správcovia skupiny, správcovia používateľov a vlastníci skupiny.
5. Ak uplynula platnosť skupiny v Office 365, odstráni sa a môže sa obnoviť až 30 dní pred trvalým odstránením. Po trvalom odstránení sa skupina už nedá obnoviť. Ďalšie informácie o obnove skupín [nájdete tu](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Automatické obnovenie na základe aktivity**

Aktivity používateľov z SharePointu, Outlooku a tímu môžu vyvolať automatické obnovenie skupiny. Aktivity sa kontrolujú na 35 dní pred uplynutím platnosti skupiny. Ak sa počas aktuálneho životného cyklu skupiny zobrazuje aktivita, skupina sa automaticky obnoví a e-mailové oznámenia sa nebudú odosielať vlastníkom skupín.

**Časovanie oznámení pre skupiny s uplynutou platnosťou**

1. E-mailové oznámenia sa odosielajú vlastníkom skupín služieb Office 365 30 dní, 15 dní a 1 deň pred uplynutím platnosti skupiny.
2. Pri prvom nastavení uplynutia platnosti budú všetky skupiny, ktoré sú staršie ako interval uplynutia platnosti, nastavené na 35 dní až do uplynutia platnosti.
3. Dátum uplynutia platnosti skupiny sa vypočíta na základe dátumu obnovenia skupiny, ktorý nie je založený na dátume aktualizácie politiky. Ak sa politika uplynutia platnosti aktualizuje, dátum uplynutia platnosti sa nezmení.
4. Ďalšie informácie nájdete v téme [politiky uplynutia platnosti skupiny a obnovenie e-mailov](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) a [Obnovenie odstránenej skupiny služieb Office 365 v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Povolenie na vytvorenie skupiny**

Uistite sa, že máte oprávnenie na vytvorenie novej skupiny. Globálni správcovia môžu vypnúť vytváranie skupín na portáli Azure alebo v Accessovom paneli. Môže byť potrebné, aby správca vytvoril novú skupinu za vás alebo aby vám povolil príslušné povolenia.

1. [Vytvorenie novej skupiny a pridanie členov na portáli Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Vytvorenie skupín v prostredí PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Zakázanie vytvárania skupín v prostredí PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Spravovanie osôb, ktoré môžu vytvárať skupiny v Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Vypnutie uvítacieho oznámenia balíka Office 365 cez prostredie PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Roly spravovania služby Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Správa povolení na vytváranie skupín**

1. Globálny správcovia môžu spravovať povolenia na vytváranie skupín pre zabezpečenie alebo skupiny služieb Office 365 vytvorené na portáli Azure alebo v Accessovom paneli nastavením **používateľov môžete vytvoriť skupiny zabezpečenia v Azure portály** alebo **Používatelia môžu vytvárať skupiny v Office 365** v nastaveniach Azure portal vo **všetkých skupinách > všeobecné (nastavenia)**.
2. Môžete tiež obmedziť vytváranie skupín a vybrať skupinu používateľov, ak máte licenciu služby Azure AD P1 Premium.

**Vypnutie uvítacieho oznámenia pre nových členov skupiny v Office 365**

Uvítacia notifikácia odoslaná používateľom, ktorí boli pridaní do skupín služieb Office 365, môže byť zakázaná nastavením `UnifiedGroupWelcomeMessageEnabled` na **hodnotu False** v prostredí PowerShell. Oboznámte sa s týmto nastavením [tu](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













