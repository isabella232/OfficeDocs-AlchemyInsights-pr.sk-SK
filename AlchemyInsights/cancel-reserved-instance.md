---
title: Zrušenie rezervácie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807990"
---
# <a name="cancelling-reservation"></a>Zrušenie rezervácie

- **Samoobslužné:** Vyhradenú inštanciu môžete zrušiť alebo vymeniť pomocou služby [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezerváciu a kliknite na položku refundácia alebo Exchange. Všimnite si, že musíte mať prístup vlastníka k objednávke rezervácie na Exchange alebo refundáciu. Prístup k rezervácii vám neumožní pokračovať v refundácii alebo výmene. Požiadajte vlastníka objednávky rezervácie, aby vám priradil prístup k objednávke rezervácie
- **Politika Exchange:** Môžete si rezervovať rezerváciu na ďalšiu rezerváciu toho istého typu – neexistujú **žiadne pokuty** na rezervačnej výmene. Celkový záväzok s novou rezerváciou by mal byť väčší ako súčet vymenených náhrad za rezerváciu a budúcich mesačných splátok (ak je to možné).
- **Politika vrátenia dane:** Súčet vývozných náhrad a zrušených budúcich platieb nemôže prekročiť $50 000 USD v 12-mesačnom priebežnom okne. V súčasnosti neúčtujeme **žiadne sankcie** za refundácie, ale mohli by sme ho účtovať na budúce refundácie.  
    **Výnimky:** Samoobslužné služby Exchange a Cancel nie sú k dispozícii pre zákazníkov v rámci vládnych podnikových zmlúv v USA
- Podpora **rozhrania API/PS/CLI** nie je k dispozícii na zrušenie a refundácie [samoobslužné výmeny a refundácie za rezervácie Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samoobslužné služby Exchange a Cancel nie sú k dispozícii pre zákazníkov v rámci vládnych podnikových dohôd v USA. Ďalšie typy predplatného na členstvo v USA vrátane Pay-as-you-go a CSP sú podporované

Ďalšie informácie: [ako sa spracúvajú vrátené a vymieňané transakcie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Ďalšie informácie: [politiky Exchange a refundácie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Ďalšie otázky: [navštívte dokumenty vyhradené inštancie](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Výmena existujúcej vyhradenej inštancie (samoobslužná)**

Rezerváciu môžete rezervovať na ďalšiu rezerváciu toho istého typu. Ak ju už nepotrebujete, môžete tiež vrátiť rezerváciu až do $50 000 USD za rok. Samoobslužné služby Exchange a Cancel nie sú k dispozícii pre zákazníkov v rámci vládnych podnikových dohôd v USA. K dispozícii sú aj iné typy predplatného na členstvo v USA vrátane Pay-as-you-go a CSP. Na výmenu alebo vrátenie existujúcej rezervácie musíte mať prístup vlastníka k objednávke rezervácie.

Nasledujúce kroky budú sprevádzať postup dokončenia transakcie

1. Prihláste sa na [portáli Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Vyberte rezervácie, ktoré chcete vrátiť, a kliknite na položku **Exchange** .
2. Vyberte produkt VM, ktorý chcete kúpiť, a zadajte množstvo. Uistite sa, že nový súčet nákupov je viac ako celkový počet vrátených [pred nákupom](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy) .
3. Kontrola a ukončenie transakcie

**Refundácia pre vyhradenú inštanciu**

Ak chcete vrátiť rezerváciu, prejdite na **Podrobnosti rezervácie** a kliknite na položku **refundácia** .

**Pre-hodnotené refundácie:**

**Príklady pre dávky a minimálne požiadavky na refundáciu a výmenu**  
Príklad rezervácie v popredí:

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

**Odporúčané dokumenty**

- [Spôsob spracovania vrátených a výmenných transakcií](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Politiky Exchange a refundácie](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)