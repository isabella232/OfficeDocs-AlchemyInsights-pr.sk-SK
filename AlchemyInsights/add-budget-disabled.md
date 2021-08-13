---
title: Prečo je tlačidlo Pridať rozpočet pre mňa vypnuté?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954694"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Prečo je tlačidlo Pridať rozpočet pre mňa vypnuté?

Ak chcete vytvoriť rozpočet, potrebujete jedno z nasledujúcich povolení:

- Management Group, Subscription, Resource Group Scopes
- Prispievateľ riadenia nákladov
- Vlastník
- Prispievateľ
- Iba podnikový zákazník: registrácia, oddelenie, rozsahy zákazníkov
- Správca registrácie (nastaviť rozpočet v rozsahu Registrácia)
- Správca oddelenia (nastavenie rozpočtu v rozsahu oddelení)
- Vlastník konta (nastaviť rozpočet v rozsahu Konto)
- Modern Customer Agreement Only: Billing Account, Billing Profile, Invoice Section Scopes
- Tvorca predplatného na Azure

**Vytvoril/-a som rozpočet, keď náklady na aktuálny mesiac už boli nadrozpočtové. Prečo sa mi nevyhodí upozornenie?**  
Ak ste už prekročili stanovenú prahovú hodnotu nákladov, keď vytvoríte rozpočet, ktorý sa nevyzná. Po začatí nového cyklu sa po narušení prahovej hodnoty spustí upozornenie.

**Kedy očakávam prijatie upozornenia, keď presiahnem jednu z definovaných prahových hodnôt upozornení na rozpočet?**  
Rozpočty sa vyhodnocujú raz za 4 hodiny. Kým údaje o používaní dosiahnu systém rozpočtov, trvá minimálne 8 hodín. Upozornenie môže po prekročenie prahovej hodnoty trvať až 12 hodín.

**Prečo je tlačidlo Počiatočný dátum vypnuté, keď vyberiem obdobie vynulovania mesiaca alebo fakturácie?**  
Rozpočty sa zosúlaďuje s aktuálnym kalendárnym mesiacom alebo aktuálnym fakturačným obdobím (v prípade, že je vybratý fakturačný mesiac). Preto sme túto hodnotu vopred vyplniť za vás.

**Prečo sa mi v tvorbe rozpočtu zobrazuje graf nákladov?**  
Pred vykreslením grafu, ktorý vám pomôže s vytváraním rozpočtu, potrebujeme údaje minimálne o 2 mesiace.

**Prečo nemôžem nastaviť rozpočet na predplatné, ktoré som práve vytvoril?**  
Po vytvorení predplatného údaje zaberú 24 až 48 hodín, kým pre ne nastavia rozpočet.

**Rozpočtové zdroje rozhrania API**

- [Rozhranie API pre rozpočty v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Poskytuje operácie na vytvorenie a aktualizáciu rozpočtov. Pomocou rozhrania BUDGETS API môžete nastaviť prahovú hodnotu rozpočtu a nastaviť, aby sa pri prístupe k tejto prahovej hodnote nastavili viaceré upozornenia, ktoré sa majú ohliť. Upozornenia môžu spustiť e-mail alebo skupinu akcií Azure a vykonať automatizáciu. Poznámka: Filtrovanie tohto rozhrania API sa nezarovnáva s filtrovaním a rozmermi rozhrania API dotazu.
- [Rozhranie API pre rozpočty v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Vytvorenie rozpočtov s väčšími možnosťami filtrovania nákladov ako v1. Filtrovanie sa zarovná podľa zmluvy používanej v rozhraní API dotazov a dimenzií. Toto je odporúčané rozhranie API pre rozpočty na posúvanie ďalej.
- [Rozmery:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Poskytuje operácie na získanie podporovaných dimenzií pre vaše použitie v rôznych rozsahoch. Pomocou rozhrania API dimenzií môžete načítať zoznam dimenzií, ktoré možno použiť ako vstupy na generovanie dotazov pomocou rozhrania API dotazu.
- [Dotaz:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Poskytuje operácie na získanie agregovaných údajov o nákladoch a používaní na základe dotazu, ktorý poskytnete. Pomocou rozhrania Query API môžete zadať požadované filtrovanie, zoradenie a zoskupenie podľa všetkých dostupných dimenzií (ktoré sú prístupné prostredníctvom rozhrania API dimenzií).

**Predpokladané náklady**

**Prečo sa mi v analýze nákladov prognózy mojich nákladov zobraziť?**  
Prognózy prognózy môžu pre vás v analýze nákladov chýbať z viacerých dôvodov, niektoré z nich sú nasledovné:

1. Ak sú vaše údaje o nákladoch menšie ako 10 dní, graf prognózy sa načíta. Model vyžaduje minimálne 10 dní posledných údajov o nákladoch na presné prognózy.
2. Ak ste vybrali historické dátumy, graf s prognózou sa nebude zobrazovať. Vyberte rozsah dátumov s budúcimi dátumami na zobrazenie grafu prognózy
3. Ak vaše konto používa viacero mien, graf prognózy bude projekt iba pre všetky náklady v USD.

**Prečo sa pri zmenách v zdrojoch nemení prognóza?**  
Model prognózy vyžaduje, aby zmeny v konte boli vykonané niekoľko dní a na základe zmien v zdrojoch sa okamžité prognózy nevymýšli.  
V prípade väčších krokov zvýšenia alebo zníženia zdrojov bude úpravu týchto zmien v prípade anomálií trvať o niečo dlhšie

**Prečo sa moja prognóza zväčšuje po zakúpení rezervácie alebo služby Marketplace?**  
Model prognózy zohľadňuje skutočné náklady a nezahŕňa použitie a nákup samostatne. Pri jednonákupe model po 10 dňoch zníži prognózy, aby sa u vás zrazu zvýšilo náklady

**Chcem zobraziť prognózy pre jednu dimenziu (napr. Meter)**  
Prognóza momentálne podporuje celkové prognózy nákladov, nie pre jednotlivé metre. Teda, keď sa dimenzia "Zoskupiť podľa" zobrazí ako súčet všetkých položiek dimenzie.

**Odporučené dokumenty**

- [Čo je Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Osvedčené postupy riadenia nákladov služby Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analýza nákladov a výdavkov](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Skúmanie a analýza nákladov pomocou analýzy nákladov](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Ceny](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kontrola nákladov v analýze nákladov](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videokuvor: Vytvorenie rozpočtu na portáli Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Predpoklady na zobrazenie a prispôsobenie rozpočtov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Vytváranie a správa rozpočtov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurácia automatizácie pomocou rozhrania Azure Action Groups a Budgets API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Používanie upozornení na náklady na sledovanie používania a výdavkov](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Osvedčené postupy riadenia nákladov](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Videoku kurzy**

- [Vytvorenie rozpočtu na portáli Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Riadenie nákladov pomocou rozhrania API pre rozpočty a skupín akcií](https://go.microsoft.com/fwlink/?linkid=2147038)