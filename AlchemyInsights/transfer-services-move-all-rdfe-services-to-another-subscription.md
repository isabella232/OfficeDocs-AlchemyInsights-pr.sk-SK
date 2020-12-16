---
title: Prenos služieb – presun všetkých služieb RDFE do iného predplatného
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692176"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Prenos služieb – presun všetkých služieb RDFE do iného predplatného

**Premiestnenie zdrojov**

Azure zdroje je možné premiestniť do iného predplatného alebo skupiny zdrojov v rámci toho istého predplatného pomocou platformy Azure Portal, Azure PowerShell, Azure CLI alebo rozhrania REST API na presun zdrojov.

Skôr ako budete môcť presúvať zdroje, pozrite si tému:

- [Kontrolný zoznam pred presunom zdrojov](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Služby, ktoré je možné premiestniť](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Overenie premiestnenia](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Premiestnenie poradenstva pre služby](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Ak chcete premiestniť existujúce zdroje do inej skupiny zdrojov alebo predplatného, môžete použiť:

- [Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Kurz: [premiestnenie zdrojov Azure do inej skupiny zdrojov alebo predplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Riešenie chýb v službe Azure Resource Manager**

Pozrite si články nižšie a získajte informácie o niektorých bežných chybách nasadenia Azure a prijímanie informácií na ich vyriešenie. Ak nemôžete nájsť kód chyby chyby nasadenia, pozrite si tému [Vyhľadanie kódu chyby](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Riešenie chýb nasadenia](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Riešenie problémov so sťahovaním Azure zdrojov do novej skupiny zdrojov alebo predplatného](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Všimnite si, že ak chcete inovovať svoje predplatné Azure, ako napríklad prechod z bezplatnej platby na Pay-as-you-go, budete musieť skonvertovať predplatné.

- Ak chcete inovovať bezplatnú skúšobnú verziu, pozrite si tému [Inovácia bezplatnej skúšobnej verzie alebo predplatného služby Microsoft Imagine Azure na zaplatenie predplatného](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Ak chcete zmeniť konto Pay-as-you-go, pozrite si tému [Zmena predplatného v službe Azure Pay-as-you-go do inej ponuky](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Pridanie alebo priradenie predplatného Azure k nájomníkovi služby Azure Active Directory:**

1. Prihláste sa a vyberte predplatné, ktoré chcete použiť zo [stránky predplatné na portáli Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Vyberte položku **zmeniť adresár**.
3. Skontrolujte všetky zobrazené upozornenia a potom vyberte položku **zmeniť**.
4. Adresár sa zmení na predplatné a zobrazí sa hlásenie o úspechu.
5. Pomocou prepínača *adresára* prejdite do nového adresára. Ak chcete, aby sa všetko zobrazilo správne, môže trvať až 10 minút.

**Odporúčané dokumenty**

- [Prenos vlastníctva predplatného Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Premiestnenie zdrojov do novej skupiny zdrojov alebo predplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Správa zdrojov pomocou služby Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
