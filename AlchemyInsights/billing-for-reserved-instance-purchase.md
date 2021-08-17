---
title: Fakturácia za nákup rezervovanej inštancie
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
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104035"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturácia za nákup rezervovanej inštancie

Nákup rezervovanej inštancie sa účtuje spôsobom úhrady viazaným na predplatné, ktorý vyberiete v čase zakúpenia. Typ predplatného musí byť zmluva Enterprise (číslo ponuky: MS-AZR-0017P), Pay-As-You-Go (číslo ponuky: MS-AZR-0003P), zmluva spoločnosti Microsoft so zákazníkom alebo CSP.

- V prípade predplatného Enterprise sa poplatky odpočítajú zo zostatku peňažného záväzku danej registrácie alebo sa účtujú ako prekročená suma
- V prípade priebežného predplatného Pay-As-You-Go sa poplatky účtujú na kreditnú kartu alebo sa použije spôsob platby na faktúru v rámci predplatného

**Zrušenie rezervácie**

- **Samoobslužné služby:** Rezervovanú inštanciu môžete zrušiť alebo vymeniť sami pomocou [portálu Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vyberte rezerváciu a kliknite na refundáciu alebo výmenu. Na výmenu alebo refundáciu je potrebné mať prístup vlastníka na objednávke rezervácie. Prístup len k rezervácii vám neuplatí na refundáciu ani výmenu. Požiadajte vlastníka objednávky rezervácie, aby vám vlastníkovi dal prístup k objednávke rezervácie
- **Exchange politiky:** Rezerváciu si môžete vymeniť na inú rezerváciu rovnakého typu, pri výmeny rezervácií sa **u** vás nič u vás nebude chovať. Celková viazanosť s novou rezerváciou by mala byť väčšia ako súčet refundácie rezervácie a budúce mesačné platby (ak je k dispozícii)
- **Politika refundácie:** Suma refundácie a zrušené budúce platby nemôžu presiahnuť 50 000 USD v 12-mesačnom okne. Momentálne sa **nám neplatia žiadne aktuálne informácie o** refundáciách, ale mohli by sme ju účtovať za budúce refundácie

**Výnimky:** Samoobslužná výmena a zrušenie možnosti nie sú k dispozícii pre zákazníkov zo štátnej zmluva Enterprise USA

- **Podpora rozhrania API, PS alebo CLI** nie je k dispozícii pri zrušení a refundáciách [Samoobslužné burzy a refundácie za Rezervácie v Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samoobslužná výmena a zrušenie možnosti nie sú k dispozícii pre zákazníkov zo štátnej zmluva Enterprise USA. Podporované sú aj iné typy predplatného us Government vrátane predplatného Pay-As-You-Go a CSP

Ďalšie informácie: [Ako sa spracúvajú](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) transakcie vrátenia a výmeny Ďalšie informácie: Exchange a politiky [refundácie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Ďalšie otázky: [Návšteva vyhradených dokumentov inštancií](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange rezervovanej inštancie (samoobslužná)**

Rezerváciu si môžete vymeniť na inú rezerváciu rovnakého typu. Ak už rezerváciu nepotrebujete, môžete tiež refundovať až do 50 000 USD ročne. Samoobslužná výmena a zrušenie možnosti nie sú k dispozícii pre zákazníkov zo štátnej zmluva Enterprise USA. Podporované sú aj iné typy predplatného us Government vrátane služieb Pay-As-You-Go a CSP. Ak si chcete vymeniť alebo refundovať existujúcu rezerváciu, musíte mať na objednávke rezervácie prístup vlastníka.

Nasledujúce kroky budú príručky pre postup na dokončenie transakcie

1.Prihláste sa na [portál Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vyberte rezervácie, ktoré chcete refundovať, a kliknite **na položku Exchange** 2.Vyberte produkt VM, ktorý chcete kúpiť, a zadajte množstvo. Uistite sa, že celková veľkosť nového nákupu je väčšia ako celková hodnota vrátenej sumy Určenie [správnej veľkosti pred zakúpení](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Skontrolujte a dokončite transakciu

**Refundácia za rezervovanú inštanciu**

Ak chcete refundovať rezerváciu, prejdite na položku **Podrobnosti rezervácie** a kliknite na položku **Refundovať**

**Pro refundácia s hodnotením:**

**Pro a minimálne príklady požiadaviek na refundáciu** a výmenu Príklad rezervácie vopred:

- Jednoročné obdobie RI ste si kúpili za 120 EUR 1. januára
- 7. apríla budete chcieť refundovať alebo si vymeniť túto rezerváciu
- Keďže rezervácie je 97 dní v živom okolí, získate (1 – 97/365) * 120 USD späť. (t. j. 88,1 $). Momentálne nie sú k dispozícii žiadne ohodné refundácie
- Pri výmene by mala byť nová kúpa väčšia ako 88,1 $
- Momentálne nie sú k dispozícii žiadne ohodné refundácie

**Príklad rezervácie plánu fakturácie:**

- Zakúpite si jednoročné obdobie RI za 10 USD mesačne
- 7. apríla budete chcieť refundovať alebo si vymeniť túto rezerváciu
- Keďže posledná platba sa stala 7 dní, získate (1-7/31) * 10 USD späť. (t. j. 7,74 $)
- Budúce zrušené platby sú 80 EUR. Momentálne nie sú k dispozícii žiadne ohodné refundácie
- Pri zrušení platby sa odpočíta suma 87,74 USD od limitu refundácie 50 000 USD.
- V prípade výmeny by celková hodnota nového nákupu mala byť väčšia ako 87,74 $

**Nie je možné zobraziť faktúru za posledné fakturačné obdobie**

Niekoľko možných dôvodov, prečo sa faktúra nemusí zobraziť:

- Pri predplatnom máte mesačnú sumu kreditu, ktorú ste neprekročili alebo máte k dispozícii bezplatnú skúšobnú verziu. Faktúra sa vygeneruje len vtedy, keď máte peniaze
- Od dňa, kedy ste si Azure predplatil, je to menej ako 30 dní
- Faktúra ešte nie je vygenerovaná. Počkajte do konca fakturačného obdobia
- Ak nie ste správcom kont, staršie faktúry vám nemusia byť k dispozícii

**Stiahnite si faktúru z portálu Azure (.pdf)**

- Výber predplatného zo stránky [Predplatné na](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) portáli Azure ako používateľ s prístupom [k faktúre](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Výber **faktúr**
- Kliknutím **na položku** Stiahnuť faktúru zobrazíte kópiu PDF faktúry. Ak sa zobrazí **správa Nie** je k dispozícii, pozrite si časť Prečo sa mi [faktúra za posledné fakturačné obdobie nevidím?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Prijatie faktúry e-mailom (.pdf)**

- Zo stránky Predplatné vyberte [svoje](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) predplatné. Kliknite **na položku Faktúry a** potom na položku Odoslať faktúru e-mailom
- Kliknite **na položku Vyjadrite** explicitný súhlas s podmienkami. Budete musieť prihlásiť pre každé predplatné, ktoré vlastníte

Poznámka: Ak po dokončení týchto krokov dostanete e-mail, skontrolujte správnosť e-mailovej adresy v predvoľbách [komunikácie vo svojom profile.](https://account.windowsazure.com/profile)

**Stiahnutie údajov o používaní z portálu Azure**

- Prihláste sa [do Centra kont Azure](https://account.windowsazure.com/Subscriptions) ako správca [konta](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Vyberte predplatné, pre ktoré chcete zobraziť informácie o faktúre a používaní
- Vyberte **položku História fakturácie**
- Výberom **položky Zobraziť** aktuálny výpis zobrazíte odhad poplatkov v čase, keď bol odhad vygenerovaný
- Ak **chcete stiahnuť denné** údaje o používaní vo formáte CSV, vyberte položku Stiahnuť používanie. Ak sú k dispozícii dve verzie, stiahnite si verziu 2

Ďalšie otázky: [Návšteva dokumentov vyhradených inštancií](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Odporučené dokumenty**

- [Základy fakturácie](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informácie o spôsobe aplikovania zľavy na rezervovanú inštanciu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Stiahnutie alebo zobrazenie faktúry za Azure a denných údajov o používaní](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informácie o spôsobe aplikovania zľavy na rezervovanú inštanciu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informácie o používaní rezervovanej inštancie pre predplatné služby Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Informácie o používaní rezervovanej inštancie pre registráciu podniku](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows softvéru, ktoré nie sú súčasťou vyhradených inštancií](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Vyhradené inštancie v programe Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)