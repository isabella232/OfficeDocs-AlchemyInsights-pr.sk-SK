---
title: Prenos vlastníctva služby Azure fakturácie
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922169"
---
# <a name="transfer-azure-billing-ownership"></a>Prenos vlastníctva služby Azure fakturácie

Prihláste sa na [portáli Azure](https://portal.azure.com/) ako správca konta na fakturáciu s predplatným, ktoré chcete preniesť. Ak si nie ste istí, či ste a ste správcom, alebo ak potrebujete zistiť, kto je, pozrite si tému [určenie správcu fakturácie konta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Vyhľadávanie v **správe nákladov + Fakturácia**.
- Vyberte položku **predplatné** z ľavej tably. V závislosti od Accessu možno budete musieť vybrať rozsah fakturácie a potom **predplatné** alebo **predplatné Azure**.
- Vyberte položku **previesť vlastníctvo fakturácie** na predplatné, ktoré chcete preniesť
- Zadajte e-mailovú adresu používateľa, ktorý je správcom fakturácie konta, ktorý bude novým vlastníkom predplatného a potom vyberte položku **Odoslať žiadosť o prenos** .
- Používateľ dostane e-mail s pokynmi na kontrolu žiadosti o prenos. Ak chcete schváliť žiadosť o prenos, používateľ vyberie prepojenie v e-maile a postupujte podľa pokynov.

**Poznámka** : Ak prenesiete vlastníctvo fakturácie vášho predplatného na konto používateľa v inom nájomníkovi služby Azure AD, všetky priradenia [riadenia prístupu na základe rolí (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)na spravovanie zdrojov v predplatnom sa natrvalo odstránia. Iba nový vlastník bude mať prístup k správe zdrojov v predplatnom. Ďalšie informácie nájdete v téme [prenos predplatného používateľovi v inom nájomníkovi služby Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Odporúčané dokumenty**

- [Prenos vlastníctva fakturácie prostredníctvom Azure predplatného na iné konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Informácie o prenose vlastníctva fakturácie pre predplatné Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Prenos Visual Studio, Microsoft Partner Network (MPN) a Pay as you go dev/test predplatného](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Najčastejšie otázky o prenose vlastníctva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Riešenie problémov s vlastníctvom prenosu](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
