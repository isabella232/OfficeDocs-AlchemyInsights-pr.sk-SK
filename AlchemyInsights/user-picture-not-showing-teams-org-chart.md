---
title: User picture not showing in Microsoft Teams organization chart
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792885"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>User picture not showing in Microsoft Teams organization chart

Ak v organizačnej schéme chýba profilová fotografia jedného alebo viacerých osôb vo vašej organizácii, je možné, že nastavenie **ShowInAddressLists** je nastavené na hodnotu **False:**

1. Prejdite na Centrum spravovania služby Microsoft 365 > [**Aktívni používatelia**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)a vyberte používateľa, ktorý má chýbajúcu fotografiu. 
1. Vyberte kartu **Pošta** a uistite sa, že možnosť **Zobraziť v globálnom zozname adries** je nastavená na možnosť **Áno.** 

Ak nastavenie **možnosti ShowInAddressLists** na áno nefunguje, skontrolujte toto: 

- Používateľ môže byť skrytý v zozname príjemcov v Exchange. Ďalšie informácie nájdete v téme [Správa zoznamov adries v Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Používateľ môže byť skrytý v zozname adries v Azure Active Directory. Ďalšie informácie nájdete v téme [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
