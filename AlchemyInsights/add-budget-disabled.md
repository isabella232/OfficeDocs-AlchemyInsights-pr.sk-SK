---
title: Prečo je pre mňa tlačidlo Pridať rozpočet vypnuté?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807669"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Prečo je pre mňa tlačidlo Pridať rozpočet vypnuté?

Ak chcete vytvoriť rozpočet, budete potrebovať niektoré z nasledujúcich povolení:

- Skupina správy, predplatné, rozsahy skupiny zdrojov
- Prispievateľ správy nákladov
- Vlastník
- Prispievateľ
- Iba podnikový zákazník: registrácia, oddelenie, rozsahy kont
- Správca registrácie (nastavte rozpočet na rozsah registrácie)
- Správca oddelenia (nastaviť rozpočet na oddelenie rozsahu)
- Vlastník konta (nastavte rozpočet na rozsah konta)
- Iba moderná zmluva o zákazníkovi: fakturačné konto, profil fakturácie, rozsahy sekcie fakturácie
- Tvorca predplatného Azure

**Vytvoril som rozpočet, keď moje náklady na aktuálny mesiac už boli viac než rozpočtové. Prečo sa mi nezobrazilo upozornenie?**  
Ak ste už prekročili určitú prahovú hodnotu nákladov, keď vytvoríte rozpočet, ktorý upozornenie nebude k požiaru. Po začatí nového cyklu, ak porušíte prahovú hodnotu, potom sa upozornenie spustí.

**Kedy mám očakávať, že dostanem upozornenie, keď prekročím jeden z mojich definovaných prahov upozornení na rozpočet?**  
Rozpočty sa hodnotia každých 4 hodín. Ak chcete, aby sa údaje o používaní dosiahli do systému rozpočtov, trvá minimálne 8 hodín. Na základe tohto upozornenia môže trvať až 12 hodín, kým neprekročíte prahovú hodnotu.

**Prečo je tlačidlo dátum začatia vypnuté, keď vyberiete obdobie obnovenia mesiaca alebo fakturácie mesiaca?**  
Rozpočtové prostriedky sú zarovnané na aktuálny kalendárny mesiac alebo aktuálne fakturačné obdobie (v prípade, že je vybratá položka Fakturácia month). Preto sme pred vyplnením tejto hodnoty.

**Prečo sa nezobrazuje graf mojich nákladov v rámci vytvárania rozpočtu?**  
Na vykreslenie grafu, ktorý vám pomôže s vytvorením rozpočtu, potrebujeme minimálne 2 mesiace údajov o nákladoch.

**Prečo nemôžem nastaviť rozpočet na predplatné, ktoré som práve vytvoril?**  
Po vytvorení predplatného údaje trvá 24-48 hodín na spracovanie pred nastavením rozpočtu.

**Zdroje informácií o rozpočte API**

- [Rozpočet API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): poskytuje operácie na vytváranie a aktualizáciu rozpočtov. Pomocou rozhrania API rozpočty môžete nastaviť rozpočtovú prahovú hodnotu a nakonfigurovať viacero upozornení na oheň pri prístupe k tejto hranici. Výstrahy môžu vyvolať e-maily alebo akcie skupiny Azure na vykonávanie automatizácie. Poznámka: filtrovanie tohto rozhrania API sa nezarovná s filtrovaním a rozmermi API dotazov.
- [Rozpočet API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): vytvorenie rozpočtov s vyššou možnosťou filtrovania nákladov ako v1. Filtrovanie sa zarovná k zmluve použitej v našich dotazoch a dimenziách API. Toto je odporúčaný rozpočet API na používanie posúvania dopredu.
- [Dimenzie](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): poskytuje operácie na získanie podporovaných dimenzií používania v rámci rôznych rozsahov. Pomocou rozhrania API dimenzie môžete získať zoznam dimenzií, ktoré možno použiť ako vstupy na generovanie dotazov pomocou rozhrania API dotazov.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): poskytuje operácie na získanie agregovaných nákladov a údajov o používaní na základe vami poskytnutých dotazov. Pomocou rozhrania API dotazu môžete zadať požadované filtrovanie, zoradenie a zoskupenie všetkých dostupných dimenzií (prístupných z rozhrania API pre dimenzie).

**Prognózované náklady**

**Prečo sa v analýze nákladov nezobrazujú prognózy pre moje náklady?**  
Existuje viacero dôvodov, prečo môže byť v analýze nákladov v rámci analýzy nákladov chýbajúca prognóza, niektoré z nich sú nasledovné:

1. Ak je váš údaj o nákladoch menší ako 10 dní, prognózovaný graf sa nenačíta. Model vyžaduje minimálne 10 dní najnovších údajov o nákladoch na presné výčnelky
2. Ak ste vybrali možnosť historické dátumy, nezobrazí sa prognózovaný graf. Vyberte rozsah dátumov s budúcimi dátumami, ktoré sa majú zobraziť v prognóze grafu.
3. Ak máte vo svojom konte viaceré meny, v prognózovanom grafe sa zobrazia iba náklady na projekt za všetky náklady v USD.

**Prečo sa po vykonaní zmien v mojich zdrojoch nezmení prognóza?**  
V modeli Forecast sa vyžaduje niekoľko dní, aby sa zohľadnili zmeny v konte a nevykonali sa okamžité projekcie na základe zmeny zdrojov.  
Pri väčších krokoch na zvýšenie alebo zníženie zdrojov bude model trvať o niečo dlhšie, kým sa tieto zmeny prispôsobia anomáliám.

**Prečo sa po zakúpení rezervácie alebo trhoviska zvýšila moja predpoveď počasia?**  
V modeli Forecast sa považuje za skutočné náklady a nevzťahuje sa na použitie a zakúpenie samostatne. Pri jednorazovom nákupe bude model klesať po 10 dňoch, aby sa zohľadnilo náhle zvýšenie nákladov

**Chcem zobraziť prognózy pre jeden rozmer (napr. Meter**  
Prognóza v súčasnosti podporuje celkový odhad nákladov a nie pre jednotlivé elektromery. Pri zoskupení podľa dimenzie bude mať projekcie celkový súčet všetkých položiek v dimenzii.

**Odporúčané dokumenty**

- [Čo je spravovanie nákladov Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najvhodnejšie postupy spravovania nákladov Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analýza nákladov a výdavkov](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Skúmanie a analýza nákladov pomocou analýzy nákladov](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Správa nákladov Azure: ceny](https://azure.microsoft.com/services/cost-management/#pricing)
- [Revízia nákladov na analýzu nákladov](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video kurz: vytvorenie rozpočtu na portáli Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Predpoklady na zobrazenie a prispôsobenie rozpočtov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Vytváranie a správa rozpočtov](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurácia automatizácie pomocou Azure Action groups a rozpočty API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Používanie upozornení o nákladoch na monitorovanie používania a výdavkov](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najvhodnejšie postupy spravovania nákladov](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Výukové videá**

- [Vytvorenie rozpočtu na portáli Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Správa nákladov pomocou rozhrania API a akčných skupín pre rozpočty](https://go.microsoft.com/fwlink/?linkid=2147038)