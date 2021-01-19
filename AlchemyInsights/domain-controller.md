---
title: Radič domény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901313"
---
# <a name="domain-controller"></a>Radič domény

**Nie je možné povoliť AAD-DS alebo nasadenie zlyháva**

Ak chcete vyriešiť problém služby Azure AD Domain (AAD-DS), ktorý nie je povolený alebo nie je možné nasadiť, vykonajte tieto kroky:

1. Ak používate už existujúcu virtuálnu sieť, pozrite si NSG pravidlá, ktoré blokujú porty potrebné na synchronizáciu v rámci AAD-DS na portáli https://aka.ms/aadds-networking .
2. Skontrolujte, či sa v tejto príručke na riešenie problémov, ktorá je k dispozícii, zobrazí chybové hlásenie  https://aka.ms/aadds-troubleshoot-enable .
3. Skúste nasadiť služby Azure AD Domain Services v novej virtuálnej sieti.
4. Postupujte podľa pokynov Začíname s nasadením AAD-DS, ktoré je k dispozícii na lokalite [tutorial na vytvorenie služieb Azure AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ak máte problémy s nasadením služieb Azure AD Domain, prečítajte si tému [Riešenie problémov s doménou služby Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) na vyriešenie bežných chýb, ktoré vám pomôžu pri opätovnom práci. 

**AAD-DS sa nedá vypnúť**

AAD-DS nie je možné pozastaviť. Ak chcete prestať používať spravovanú doménu, musí byť odstránená.

Ak sa vyskytnú problémy, riešenie bežných chybových hlásení a súvisiace kroky na riešenie problémov, ktoré vám pomôžu znova začať pracovať, pozrite si tému [Riešenie problémov s doménovou službou Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
