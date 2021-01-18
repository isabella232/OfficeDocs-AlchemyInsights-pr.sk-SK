---
title: Priradenie skupín k úlohe Azure AD
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
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885397"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Priradenie skupín k úlohe Azure AD

Ak chcete priradiť skupinu Azure AD so zdrojom autority v službe Azure AD na rolu Azure AD, vykonajte tieto kroky:

1. Vytvorenie novej skupiny – vytvorenie novej skupiny:

    a. Prihláste sa do centra spravovania služby Azure AD s **privilegovaným správcom roly** alebo povoleniami **globálneho správcu** .
    b. Vyberte položku **Azure Active Directory > skupiny > všetky skupiny > novú skupinu**.
    c. Vytvorte skupinu.

2. Priraďte rolu skupine buď počas vytvárania skupiny alebo po vytvorení skupiny.

    a. Ak chcete skupine priradiť rolu v čase vytvárania skupiny, zapnite funkciu prepnutia **funkcií Azure AD môže byť priradená skupine** a vytvorte skupinu.
    b. Ak chcete priradiť rolu k skupine po jej vytvorení, prejdite na kartu **priradené roly** pre novo vytvorenú skupinu a priraďte rolu skupine.  

**Spravovanie členstva v skupine, ktorá je priradená k úlohe Azure AD**

Ak chcete zabrániť zvýšeniu počtu privilégií, na základe predvoleného nastavenia môžu členovia skupiny, ktorá je priradená k úlohe, upravovať iba privilegovaní správcovia rolí a globálni správcovia. Môže sa však rozhodnúť priradiť vlastníkovi takejto skupiny a delegovať túto úlohu.

Ďalšie informácie o priraďovaní cloudových skupín k funkciám Azure AD nájdete v téme [Priradenie ROLÍ reklamy skupine cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Ďalšie informácie o riešení problémov s rolami priradenými k cloudovým skupinám nájdete v téme [Riešenie problémov priradených k cloudovým skupinám](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





