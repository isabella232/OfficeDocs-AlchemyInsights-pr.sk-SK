---
title: Prenos vlastníctva na fakturáciu v Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036111"
---
# <a name="transfer-azure-billing-ownership"></a>Prenos vlastníctva na fakturáciu v Azure

Prihláste sa na [portáli Microsoft Azure](https://portal.azure.com/) ako správca fakturačného konta s predplatným, ktoré chcete preniesť. Ak si nie ste istí, či ste správcom, alebo ak potrebujete zistiť, kto ním je, pozrite si tému [Určenie správcu fakturácie konta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Vyhľadajte _Cost Management + Billing_ (Správa nákladov a fakturácia).
1. Na ľavej table vyberte položku **Subscriptions** (Predplatné). V závislosti od prístupu je možné, že budete musieť vybrať rozsah fakturácie a potom položku **Subscriptions** (Predplatné) alebo **Azure subscriptions** (Predplatné Azure).
1. Vyberte položku **Transfer billing ownership** (Prenos vlastníctva na fakturáciu) pre predplatné, ktoré chcete preniesť.
1. Zadajte e-mailovú adresu používateľa, ktorý je správcom fakturácie konta, ktoré bude novým vlastníkom predplatného, a potom vyberte položku **Send transfer request** (Odoslať žiadosť o prenos).
1. Používateľ dostane e-mail s pokynmi na kontrolu žiadosti o prenos. Na schválenie žiadosti o prenos, používateľ vyberie prepojenie v e-maile a postupuje podľa pokynov.

Ak prenesiete vlastníctvo na fakturáciu svojho predplatného na používateľské konto iného nájomníka služby Azure AD, všetky priradené úlohy [riadenia prístupu na základe rolí (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) na spravovanie prostriedkov v rámci predplatného sa natrvalo odstránia. Prístup na spravovanie prostriedkov v rámci predplatného bude mať iba nový vlastník. Ďalšie informácie o postupe zmeny adresára predplatného nájdete v téme [Prenos predplatného na používateľa v inom nájomníkovi služby Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Dôležité dôsledky pre vaše faktúry**_: Ak ste preniesli vlastníctvo na fakturáciu predplatného služby Azure, poplatky budú alikvótne. K faktúram budete mať prístup podľa nasledujúcich krokov:  

1. Vyberte predplatné na  [stránke Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)  (Predplatné) na portáli Microsoft Azure ako  [používateľ s prístupom k faktúram](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) a potom vyberte položku  **Invoices** (Faktúry).
1. Ak chcete zobraziť kópiu faktúry vo formáte PDF, kliknite na položku  **Download Invoice**  (Stiahnuť faktúry). Ak sa zobrazí hlásenie  _Not available_ (Nie je k dispozícii), pozrite si tému  [Prečo sa nezobrazuje faktúra za posledné fakturačné obdobie?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Môžete tiež zobraziť denné používanie kliknutím na **fakturačné obdobie** a získať súbor s faktúrou vo formáte PDF a kópiu súboru s podrobným prehľadom denného používania (.CSV). Ďalšie informácie nájdete v téme  [Získanie údajov o fakturácii a používaní](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Odporučené dokumenty**

- [Prenos vlastníctva na fakturáciu za predplatné služby Azure na iné konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informácie o prenose vlastníctva na fakturáciu za predplatné služby Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Prenos predplatných Visual Studio, Microsoft Partner Network (MPN) a Pay as you go Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos vlastníctva – najčastejšie otázky](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Riešenie problémov s prenosom vlastníctva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
