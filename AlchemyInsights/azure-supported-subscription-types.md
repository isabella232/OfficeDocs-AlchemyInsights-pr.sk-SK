---
title: Podporované typy predplatného
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
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072175"
---
# <a name="supported-subscription-types"></a>Podporované typy predplatného

Pred tým, ako budete pokračovať, skontrolujte podporované typy predplatného.

[Podporované typy predplatného](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prenos vlastníctva na fakturáciu**

Portál Microsoft Azure [ ako správca konta](https://ms.portal.azure.com/) fakturačného konta s predplatným, ktoré chcete preniesť.

- Hľadajte v časti **Cost Management + Billing** (Správa nákladov a fakturácia). Na ľavej table vyberte položku **Subscriptions** (Predplatné). V závislosti od prístupu je možné, že budete musieť vybrať rozsah fakturácie a potom položku **Subscriptions** (Predplatné) alebo **Azure subscriptions** (Predplatné Azure).
- Vyberte položku Transfer billing ownership (Prenos vlastníctva na fakturáciu) pre predplatné, ktoré chcete preniesť.
- Zadajte e-mailovú adresu používateľa, ktorý je správcom fakturácie konta, ktoré bude novým vlastníkom predplatného, a potom vyberte položku **Send transfer request** (Odoslať žiadosť o prenos).
- Používateľ dostane e-mail s pokynmi na kontrolu žiadosti o prenos. Na schválenie žiadosti o prenos, používateľ vyberie prepojenie v e-maile a postupuje podľa pokynov.

Poznámka: ak prenesiete vlastníctvo na fakturáciu svojho predplatného na používateľské konto iného nájomníka služby Microsoft Azure AD, všetky priradené úlohy [riadenia prístupu na základe rolí (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) na spravovanie prostriedkov v rámci predplatného sa natrvalo odstránia. Prístup na spravovanie prostriedkov v rámci predplatného bude mať iba nový vlastník. Ďalšie informácie nájdete v téme [Prenos predplatného na používateľa v inom nájomníkovi služby Microsoft Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prenos vlastníctva predplatného**

Na prenos vlastníctva predplatného je potrebné, aby prístup na základe role (RBAC) spravoval zdroje v predplatnom tak, aby stratili svoj prístup. Viac informácií o pridaní existujúceho predplatného do nájomníka nájdete v časti [Priradiť alebo pridať predplatné Azure do služby Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenos predplatného s existujúcou zostávajucou sumou z aktuálneho fakturačného cyklu nebude prenesený na nový platobný nástroj v novom konte. Jediné informácie dostupné používateľom v novom konte sú o cene vášho predplatného za minulý mesiac. Zbytok využitia a história fakturácie sa s predplatným neprenesú.
- Prenos vlastníctva predplatného pre predplatné zmluvy Enterprise (EA) je aktuálne podporovaný iba na portáli Enterprise Agreement Portal.
- Prenos predplatného založeného na kredite ako Visual Studio, BizSpark, Microsoft Partner Network na nového používateľa na prijatie požiadavku na prenos vyžaduje licenciu Visual Studio/Microsoft Partner Network.
- Všetky zdroje ako virtuálne počítače, disky a webové lokality sa úspešne prenesú na nové konto. Nasledovné zdroje mohli byť pri prenose predplatného medzi nájomníkmi zasiahnuté:

**Služby Microsoft Azure Active Directory Domain Services**

Azure Key Vaults

- [Používatelia a databázy súvisiace s SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) mohli byť zasiahnuté najmä vtedy, ako zákazník používa overovanie prepojené so službou Azure Active Directory
- **Služby aplikácií** konfigurované s overením služby Azure Active Directory mohlo byť zasiahnuté
- Kontá **tímovej služby Visual Studio** Team pripojené s predplatným Azure môžu dočasne stratiť prístup, keď sa zruší pripojené predplatné Azure

**Odporučené dokumenty**

Kroky po prijatí vlastníctva predplatného:

- Na udržania vlastníctva predplatného, ale zmeny typu predplatného si pozrite tému: [Prechod na inú ponuku s predplatným Azure](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos predplatných Visual Studio, Microsoft Partner Network (MPN) a Pay as you go Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos vlastníctva predplatného predplatných zmluvy Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Prenos vlastníctva – najčastejšie otázky](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Riešenie problémov s prenosom vlastníctva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)