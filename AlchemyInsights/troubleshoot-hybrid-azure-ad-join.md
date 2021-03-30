---
title: ;Riešenie problémov s pripojením k službe Hybrid Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401922"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>;Riešenie problémov s pripojením k službe Hybrid Azure AD

Dôrazne odporúčame zabezpečiť, aby zariadenie malo prístup ku koncovým bodom registrácie zariadenia v rámci systémového konta pomocou skriptu [Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Ak nastavujete registrácie zariadení po prvýkrát, nezabudnite si prečítať tému [Úvod do správy zariadení v službe Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), v ktorej zistíte, ako kontrolovať zariadenia cez službu Azure AD.
1. Ak svoje zariadenia registrujete priamo do služby Azure AD a zaregistrujete ich do služby Intune, uistite sa, že ste [nakonfigurovali službu Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a máte potrebné [licencie](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Uistite sa, že máte oprávnenie na vykonávanie operácií v službe Azure AD a lokálnej službe AD. Nastavenia registrácií zariadení môže spravovať iba globálny správca v službe Azure AD. Okrem toho, ak nastavujete automatické registrácie v lokálnej službe Active Directory, budete musieť byť správcom služby Active Directory a AD FS (ak je to potrebné).

Ďalšie podrobnosti o riešení potenciálnych problémov s pripojením Hybrid nájdete v téme [Riešenie problémov s pripojením Hybrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current), kde nájdete informácie o nastavení hybridného nasadenia služby Azure AD. Informácie o spravovaní zariadení pomocou portálu Azure Ad nájdete v témach [Nastavenie zariadení pripojených k službe Hybrid Azure AD (pripojených k lokálnej doméne)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) a [Správa zariadení pomocou portálu Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Ak chcete vyriešiť bežné problémy s pripojením k službe Hybrid Azure Active Directory (AD), pozrite si tému [Najčastejšie otázky o pripojení k službe Hybrid Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
