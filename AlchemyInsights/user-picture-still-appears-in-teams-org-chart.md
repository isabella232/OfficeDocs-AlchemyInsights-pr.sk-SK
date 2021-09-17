---
title: Obrázok používateľa sa naďalej zobrazuje v organizačnej Microsoft Teams grafe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422319"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Obrázok používateľa sa naďalej zobrazuje v organizačnej Microsoft Teams grafe

Ak boli zakázané alebo odstránené aspoň jeden jednotlivci vo vašej organizácii a ich profilová fotografia sa naďalej zobrazuje v organizačnej schéme, je možné, že nastavenie **ShowInAddressLists** je nastavené na hodnotu False: 

1. Prejdite na Centrum spravovania služby Microsoft 365 > [Aktívni používatelia a](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) vyberte používateľa s fotografiou, ktorá sa stále zobrazuje. 
1. Vyberte kartu **Pošta** a uistite sa, že možnosť **Zobraziť v globálnom zozname adries je** nastavená na možnosť **Nie.**

Ak nastavenie **možnosti ShowInAddressLists** **na** nastavenie Nie nefunguje, skontrolujte toto: 

- Používateľ sa môže zobraziť v zozname príjemcov v Exchange. Ďalšie informácie nájdete v téme [Správa zoznamov adries v Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Používateľ sa môže zobraziť zo zoznamu adries v Azure Active Directory. Ďalšie informácie nájdete v téme [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 