---
title: Transfer Services (Služby prenosu) – premiestnenie všetkých služieb ICHE do iného predplatného
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940082"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services (Služby prenosu) – premiestnenie všetkých služieb ICHE do iného predplatného

**Premiestnenie zdrojov**

Zdroje Azure je možné presunúť na iné predplatné služby Azure alebo skupinu zdrojov v rámci rovnakého predplatného pomocou portálu Azure, Azure PowerShell, Azure CLI alebo REST API na premiestňovanie zdrojov.

Pred presunením zdrojov si prečítajte tieto téme:

- [Kontrolný zoznam pred premiestnením zdrojov](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Služby, ktoré možno premiestniť](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Overenie premiestnenia](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Pokyny na presun služieb](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Ak chcete premiestniť existujúce zdroje do inej skupiny zdrojov alebo predplatného, môžete použiť:

- [Portál Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Kurz: [Premiestnenie zdrojov služby Azure do inej skupiny zdrojov alebo predplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Riešenie chýb pomocou nástroja Azure Resource Manager**

V článkoch uvedených nižšie sa dozviete o niektorých bežných chybách nasadenia služby Azure a získate informácie na ich vyriešenie. Ak nemôžete nájsť kód chyby chyby chyby pre chybu nasadenia, pozrite si časť [Vyhľadanie kódu chyby](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Riešenie chýb nasadenia](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Riešenie problémov s premiestňovaním zdrojov služby Azure do novej skupiny zdrojov alebo predplatného](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Upozorňujeme, že ak chcete inovovať svoje predplatné na Azure, napríklad prechod z bezplatnej platby na platenie prostredníctvom takéhoto predplatného, budete musieť zmeniť svoje predplatné.

- Ak chcete inovovať bezplatnú skúšobnú verziu, pozrite si článok Inovácia bezplatnej skúšobnej verzie alebo predplatné na [Microsoft Imagine Azure na verziu Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Ak chcete zmeniť konto služby Azure Pay-as-you-go, pozrite si časť Zmena predplatného služby [Azure Pay-As-You-Go na inú ponuku.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Pridanie alebo priradenie predplatného služby Azure k nájomníkovi Azure Active Directory Azure:**

1. Prihláste sa a vyberte predplatné, ktoré chcete použiť zo stránky [Predplatné na portáli Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Vyberte **položku Zmeniť adresár**.
3. Skontrolujte všetky upozornenia, ktoré sa zobrazujú, a potom vyberte položku **Zmeniť**.
4. Adresár sa pre predplatné zmení a zobrazí sa hlásenie o úspešnom prihlásení.
5. Pomocou *prepínača* adresárov prejdite do nového adresára. Zobrazenie všetkého môže trvať až 10 minút.

**Odporučené dokumenty**

- [Prenos vlastníctva predplatného na Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Premiestnenie zdrojov do novej skupiny zdrojov alebo predplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Spravovanie zdrojov pomocou portálu Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
