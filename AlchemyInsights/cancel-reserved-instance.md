---
title: Zrušenie rezervácie
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819707"
---
# <a name="cancelling-reservation"></a>Zrušenie rezervácie

- **Samoobslužné služby:** Rezervovanú inštanciu môžete zrušiť alebo vymeniť sami pomocou [portálu Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vyberte rezerváciu a kliknite na refundáciu alebo výmenu. Na výmenu alebo refundáciu je potrebné mať prístup vlastníka na objednávke rezervácie. Prístup len k rezervácii vám neuplatí na refundáciu ani výmenu. Požiadajte vlastníka objednávky rezervácie, aby vám vlastníkovi dal prístup k objednávke rezervácie
- **Politika Exchangeu:** Rezerváciu si môžete vymeniť na inú rezerváciu rovnakého typu, pri výmeny rezervácií sa **u** vás nič u vás nebude chovať. Celková viazanosť s novou rezerváciou by mala byť väčšia ako súčet refundácie rezervácie a budúce mesačné platby (ak je k dispozícii)
- **Politika refundácie:** Suma refundácie a zrušené budúce platby nemôžu presiahnuť 50 000 USD v 12-mesačnom okne. Momentálne sa **nám neplatia žiadne aktuálne informácie o** refundáciách, ale mohli by sme ju účtovať za budúce refundácie  
    **Výnimky:** Samoobslužná výmena a zrušenie možnosti nie sú k dispozícii pre zákazníkov zmluvy US Government Enterprise Agreement
- **Podpora rozhrania API, PS alebo CLI** nie je k dispozícii pri zrušení a refundáciách [Samoobslužné burzy a refundácie za Rezervácie v Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samoobslužná výmena a zrušenie možnosti nie sú k dispozícii pre zákazníkov so zmluvou US Government Enterprise. Podporované sú aj iné typy predplatného us Government vrátane predplatného Pay-As-You-Go a CSP

Ďalšie informácie: [Spôsob spracovania transakcií vrátenia a výmeny](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Ďalšie informácie: [Politiky Exchangeu a refundácie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Ďalšie otázky: [Návšteva dokumentov vyhradených inštancií](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Výmena existujúcej vyhradenej inštancie (samoobslužná)**

Rezerváciu si môžete vymeniť na inú rezerváciu rovnakého typu. Ak už rezerváciu nepotrebujete, môžete tiež refundovať až do 50 000 USD ročne. Samoobslužná výmena a zrušenie možnosti nie sú k dispozícii pre zákazníkov so zmluvou US Government Enterprise. Podporované sú aj iné typy predplatného us Government vrátane služieb Pay-As-You-Go a CSP. Ak si chcete vymeniť alebo refundovať existujúcu rezerváciu, musíte mať na objednávke rezervácie prístup vlastníka.

Nasledujúce kroky budú príručky pre postup na dokončenie transakcie

1. Prihláste sa na [portál Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Vyberte rezervácie, ktoré chcete refundovať, a kliknite na položku **Exchange**
2. Vyberte produkt VM, ktorý chcete kúpiť, a zadajte množstvo. Uistite sa, že celková veľkosť nového nákupu je väčšia ako celková hodnota vrátenej sumy [Určenie správnej veľkosti pred zakúpení](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Kontrola a dokončenie transakcie

**Refundácia za rezervovanú inštanciu**

Ak chcete refundovať rezerváciu, prejdite na položku **Podrobnosti rezervácie** a kliknite na položku **Refundovať**

**Refundácia pomernej sumy:**

**Pro-ration and minimum requirement examples for refund and exchange**  
Príklad rezervácie vopred:

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

**Odporučené dokumenty**

- [Spôsob spracovania transakcií vrátenia a výmeny](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Politiky výmeny a refundácie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)