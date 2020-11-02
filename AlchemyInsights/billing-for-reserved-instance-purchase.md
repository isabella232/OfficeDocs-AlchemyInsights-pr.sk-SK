---
title: Fakturácia na zakúpenie vyhradenej inštancie
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823169"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturácia na zakúpenie vyhradenej inštancie

Kúpa vyhradenej inštancie sa účtuje na spôsob platby spojený s predplatným, ktoré ste vybrali v čase nákupu. Typ predplatného musí byť podniková zmluva (ponuka číslo: MS-AZR-0017P), Pay-as-you-go (ponuka číslo: MS-AZR-0003P), zákaznícka zmluva spoločnosti Microsoft alebo poskytovateľ kryptografických služieb.

- Pri predplatnom podniku sa poplatky odpočítavajú zo zostatku peňažných záväzkov pri registrácii alebo sa účtujú ako nadmerné
- V prípade predplatného na Pay-as-Go sa poplatky účtujú na základe kreditnej karty alebo spôsobu úhrady faktúry na základe predplatného.

**Zrušenie rezervácie**

- **Samoobslužné:** Vyhradenú inštanciu môžete zrušiť alebo vymeniť pomocou služby [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezerváciu a kliknite na položku refundácia alebo Exchange. Všimnite si, že musíte mať prístup vlastníka k objednávke rezervácie na Exchange alebo refundáciu. Prístup k rezervácii vám neumožní pokračovať v refundácii alebo výmene. Požiadajte vlastníka objednávky rezervácie, aby vám priradil prístup k objednávke rezervácie
- **Politika Exchange:** Môžete si rezervovať rezerváciu na ďalšiu rezerváciu toho istého typu – neexistujú **žiadne pokuty** na rezervačnej výmene. Celkový záväzok s novou rezerváciou by mal byť väčší ako súčet vymenených náhrad za rezerváciu a budúcich mesačných splátok (ak je to možné).
- **Politika vrátenia dane:** Súčet vývozných náhrad a zrušených budúcich platieb nemôže prekročiť $50 000 USD v 12-mesačnom priebežnom okne. V súčasnosti neúčtujeme **žiadne sankcie** za refundácie, ale mohli by sme ho účtovať na budúce refundácie.

**Výnimky:** Samoobslužné služby Exchange a Cancel nie sú k dispozícii pre zákazníkov v rámci vládnych podnikových zmlúv v USA

- Podpora **rozhrania API/PS/CLI** nie je k dispozícii na zrušenie a refundácie [samoobslužné výmeny a refundácie za rezervácie Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samoobslužné služby Exchange a Cancel nie sú k dispozícii pre zákazníkov v rámci vládnych podnikových dohôd v USA. Ďalšie typy predplatného na členstvo v USA vrátane Pay-as-you-go a CSP sú podporované

Ďalšie informácie: [ako sa spracúvajú vrátené a vymieňané transakcie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) : Ďalšie informácie nájdete v téme [politiky Exchange a refundácie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) ďalšie otázky: [dokumenty vyhradené inštancie](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Výmena existujúcej vyhradenej inštancie (samoobslužná)**

Rezerváciu môžete rezervovať na ďalšiu rezerváciu toho istého typu. Ak ju už nepotrebujete, môžete tiež vrátiť rezerváciu až do $50 000 USD za rok. Samoobslužné služby Exchange a Cancel nie sú k dispozícii pre zákazníkov v rámci vládnych podnikových dohôd v USA. K dispozícii sú aj iné typy predplatného na členstvo v USA vrátane Pay-as-you-go a CSP. Na výmenu alebo vrátenie existujúcej rezervácie musíte mať prístup vlastníka k objednávke rezervácie.

Nasledujúce kroky budú sprevádzať postup dokončenia transakcie

1. Prihláste sa na [portáli Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervácie, ktoré chcete vrátiť, a kliknite na položku **Exchange** 2. Vyberte produkt VM, ktorý chcete kúpiť, a zadajte množstvo. Uistite sa, že nový súčet nákupov je viac ako celkový počet vrátených [pred nákupom](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Kontrola a ukončenie transakcie

**Refundácia pre vyhradenú inštanciu**

Ak chcete vrátiť rezerváciu, prejdite na **Podrobnosti rezervácie** a kliknite na položku **refundácia** .

**Pre-hodnotené refundácie:**

**Príklady pre dávky a minimálne požiadavky na refundáciu a výmenu** Príklad rezervácie v popredí:

- Zakúpite si jednoročné obdobie RI pre $120 v januári 1
- 7. apríla, ktorú chcete vrátiť alebo vymeniť túto rezerváciu
- Vzhľadom na to, že rezervácia je v 97 dňoch, dostanete (1-97/365) * $120 späť. (t.j. $88,1). V súčasnosti neexistuje žiadny trest na refundáciu
- Pri výmene by mal byť váš nový nákup väčší ako $88,1
- V súčasnosti neexistuje pokuta v prípade náhrad

**Príklad rezervácie plánu fakturácie:**

- Zakúpite jednoročné obdobie RI za $10 za mesiac
- 7. apríla, ktorú chcete vrátiť alebo vymeniť túto rezerváciu
- Od poslednej platby sa stalo 7 dní, dostanete (1-7/31) * $10 späť. (t.j. $7,74)
- Zrušené budúce platby sú $80. V súčasnosti neexistuje žiadny trest na refundáciu
- Toto zrušenie odpočíta $87,74 od ste limit vrátenia $50 000
- Pri výmene by mala byť celková hodnota nového nákupu vyššia ako $87,74

**Nie je možné zobraziť faktúru za posledné fakturačné obdobie**

Z niektorých možných dôvodov sa nemusí zobraziť faktúra:

- Máte mesačnú čiastku kreditu s predplatným, ktoré ste neprekročili, alebo máte bezplatnú skúšobnú verziu. Faktúra sa generuje len vtedy, keď dlhujete peniaze
- Je to menej ako 30 dní od dátumu, kedy ste sa pripojili k službe Azure
- Faktúra ešte nie je vygenerovaná. Počkať až do konca fakturačného obdobia
- Ak nie ste správcom konta, staršie faktúry nemusia byť k dispozícii.

**Stiahnutie faktúry zo služby Azure Portal (. pdf)**

- Výber predplatného zo stránky [predplatné](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na portáli Azure ako [používateľ s prístupom k faktúram](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Vyberte položku **faktúry**
- Ak chcete zobraziť kópiu faktúry vo formáte PDF, kliknite na položku **Stiahnuť faktúru** . Ak sa zobrazí hlásenie **nie je k dispozícii** , pozrite si tému [Prečo sa nezobrazuje faktúra za posledné fakturačné obdobie?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Príjem faktúry prostredníctvom e-mailu (. pdf)**

- Na stránke [predplatné](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) vyberte svoje predplatné. Kliknite na položku **faktúry** a potom na položku Odoslať faktúru
- Kliknite na položku **Prihlásiť** sa a vyjadrite súhlas s podmienkami. Budete sa musieť rozhodnúť pre každé predplatné, ktoré vlastníte

Poznámka: Ak sa po vykonaní týchto krokov nedostanete e-mail, skontrolujte, či je vaša e-mailová adresa správna v [predvoľbách komunikácie vo svojom profile](https://account.windowsazure.com/profile) .

**Stiahnutie údajov o používaní z portálu Azure**

- Prihláste sa do centra spravovania konta [Azure](https://account.windowsazure.com/Subscriptions) ako [správca konta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) .
- Vyberte predplatné, pre ktoré chcete fakturovať a informácie o používaní
- Vyberte položku **História fakturácie**
- Ak chcete zobraziť odhad poplatkov v čase vygenerovania odhadu, vyberte položku **Zobraziť aktuálny príkaz** .
- Vyberte položku **Stiahnuť používanie** a Stiahnite si denné údaje o používaní ako súbor CSV. Ak je k dispozícii dve verzie, Stiahnite si verziu 2

Ďalšie otázky: [navštívte dokumenty vyhradené inštancie](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Odporúčané dokumenty**

- [Základné informácie o fakturácii](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Oboznámte sa s používaním zľavy vyhradenej inštancie](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Stiahnutie alebo zobrazenie fakturačnej faktúry v službe Azure a denné údaje o používaní](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Oboznámte sa s používaním zľavy vyhradenej inštancie](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Porozumieť použitiu vyhradenej inštancie pre predplatné na Pay-as-you-go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Porozumieť použitiu vyhradenej inštancie pre registráciu podniku](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Softvérové náklady na Windows, ktoré nie sú zahrnuté v vyhradených inštanciách](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Vyhradené inštancie v programe partner Central cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)