---
title: Priradenie skupín k role služby Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036255"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Priradenie skupín k role služby Azure AD

Ak chcete k role služby Azure AD priradiť skupinu služby Azure AD so zdrojom autority v službe Azure AD, vykonajte tieto kroky:

1. Vytvorenie novej skupiny – Vytvorenie novej skupiny:

    a. Prihláste sa do Centra spravovania služby Azure AD s **privilegovaným správcom rolí** alebo **povoleniami globálneho** správcu.
    b. Vyberte **Azure Active Directory > skupiny > položku Všetky skupiny > novej skupiny**.
    c. Vytvorte skupinu.

2. Priraďte skupine rolu počas vytvárania skupiny alebo po jej vytvorení.

    a. Ak chcete k skupine priradiť rolu v čase vytvorenia skupiny, zapnite prepínač rolí služby **Azure AD,** ktoré môžu byť k tejto skupine priradené, a vytvorte skupinu.
    b. Ak chcete priradiť rolu k skupine po  jej vytvorení, prejdite na kartu Priradené roly pre novovytvorenú skupinu a priraďte skupine rolu.  

**Spravovanie členstva v skupine, ktorá je priradená k role služby Azure AD**

S cieľom zabrániť neautorizovanému výšky oprávnení môžu predvolene upravovať členstvo v skupine priradenej k role iba oprávnení správcovia rolí a globálni správcovia. Môže však priradiť vlastníka tejto skupiny a túto úlohu delegovať.

Ďalšie informácie o priraďovaní cloudových skupín k rolám služby Azure AD nájdete v téme Priradenie [rolí AD ku cloudovej skupine.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Ďalšie informácie o riešení problémov s rolami priradenými ku cloudových skupinám nájdete v téme Riešenie problémov s [rolami priradenými ku cloudovej skupine.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





