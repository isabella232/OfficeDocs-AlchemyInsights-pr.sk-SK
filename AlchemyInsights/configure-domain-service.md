---
title: Konfigurácia služby Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885688"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Nie je možné povoliť AAD-DS alebo nasadenie zlyháva

Ak chcete vyriešiť problém služby Azure AD Domain (AAD-DS), ktorý nie je povolený alebo nie je možné nasadiť, vykonajte tieto kroky:

1. Ak používate už existujúcu virtuálnu sieť, pozrite si NSG pravidlá, ktoré blokujú porty potrebné na synchronizáciu v rámci AAD-DS na portáli https://aka.ms/aadds-networking .
2. Skontrolujte, či sa v tejto príručke na riešenie problémov, ktorá je k dispozícii, zobrazí chybové hlásenie  https://aka.ms/aadds-troubleshoot-enable .
3. Skúste nasadiť služby Azure AD Domain Services v novej virtuálnej sieti.
4. Postupujte podľa pokynov Začíname s nasadením AAD – DS: [Vytvorenie a konfigurácia služieb domény AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ak máte problémy s nasadením služieb Azure AD Domain, prečítajte si tému [Riešenie problémov s doménou služby Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) na vyriešenie bežných chýb, ktoré vám pomôžu pri opätovnom práci. 

**AAD-DS sa nedá vypnúť**

AAD-DS nie je možné pozastaviť. Ak chcete prestať používať spravovanú doménu, musí byť odstránená.
Ak chcete odstrániť spravovanú doménu, pozrite si tému [Odstránenie domény služby AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



