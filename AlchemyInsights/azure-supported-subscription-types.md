---
title: Podporované typy predplatného
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
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807979"
---
# <a name="supported-subscription-types"></a>Podporované typy predplatného

Ďalšie pokyny nájdete v téme Podporované typy predplatného.

[Podporované typy predplatného](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prenos vlastníctva fakturácie**

Azure Portal ako [správca konta](https://ms.portal.azure.com/) fakturačného konta s predplatným, ktoré chcete preniesť

- Vyhľadávanie v **správe nákladov + Fakturácia** . Vyberte položku **predplatné** z ľavej tably. V závislosti od Accessu možno budete musieť vybrať rozsah fakturácie a potom **predplatné** alebo **predplatné Azure** .
- Vyberte položku previesť vlastníctvo fakturácie na predplatné, ktoré chcete preniesť
- Zadajte e-mailovú adresu používateľa, ktorý je správcom fakturácie konta, ktorý bude novým vlastníkom predplatného a potom vyberte položku **Odoslať žiadosť o prenos** .
- Používateľ dostane e-mail s pokynmi na kontrolu žiadosti o prenos. Ak chcete schváliť žiadosť o prenos, používateľ vyberie prepojenie v e-maile a postupujte podľa pokynov.

Poznámka: Ak prenesiete vlastníctvo fakturácie vášho predplatného na konto používateľa v inom nájomníkovi služby Azure AD, všetky priradenia [riadenia prístupu na základe rolí (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) na spravovanie zdrojov v predplatnom sa natrvalo odstránia. Iba nový vlastník bude mať prístup k správe zdrojov v predplatnom. Ďalšie informácie nájdete v téme [prenos predplatného používateľovi v inom nájomníkovi služby Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prenos vlastníctva predplatného**

Požiadavky na prenos vlastníctva predplatného (RBAC) na spravovanie zdrojov v predplatnom sa stratia v Accesse. Ďalšie informácie o pridaní existujúceho predplatného na nájomníka nájdete v téme [Priradenie alebo pridanie predplatného Azure do služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenos predplatného s existujúcimi nesplatenými čiastkami z aktuálneho fakturačného cyklu sa neprenesie do nového platobného nástroja v novom konte. Jedinou informáciou dostupnou pre používateľov v novom konte je cena za posledný mesiac v rámci predplatného. Zvyšok histórie používania a fakturácie sa neprenáša s predplatným.
- Predplatné na prenos vlastníctva podnikovej zmluvy (EA) je momentálne podporované len na portáli Enterprise Agreement
- Prenos predplatného s kreditnou službou, ako je napríklad Visual Studio, BizSpark, Microsoft Partner Network na nového používateľa, vyžaduje, aby bolo na prijatie žiadosti o prenos potrebné mať licenciu Visual Studio/Microsoft Partner Network.
- Všetky zdroje, ako napríklad virtuálne počítače, disky a webové lokality, sa úspešne prenášajú do nového konta. V prenose predplatného medzi nájomníkmi môžu byť ovplyvnené tieto zdroje:

**Služby Azure AD Domain**

Trezory v Azúrovom tlačidle

- [Používatelia a databázy SQL súvisia s inými používateľmi, a](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) to najmä v prípade, že zákazník používa overenie súvisiace so službou Azure Active Directory.
- Môže to mať vplyv na **služby aplikácií** nakonfigurované pomocou overenia služby Azure Active Directory
- **Tím Visual Studio** Kontá služby pripojené k predplatnému Azure môžu dočasne stratiť prístup pri zrušení pripojeného predplatného Azure

**Odporúčané dokumenty**

Kroky po prijatí vlastníctva fakturácie:

- Ak chcete zachovať vlastníctvo fakturácie, ale zmeniť typ predplatného, pozrite si tému: Zmena [predplatného Azure na inú ponuku](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos Visual Studio, Microsoft Partner Network (MPN) a Pay as you go dev/test predplatného](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos vlastníctva predplatného v rámci podnikovej zmluvy (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Najčastejšie otázky o prenose vlastníctva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Riešenie problémov s vlastníctvom prenosu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)