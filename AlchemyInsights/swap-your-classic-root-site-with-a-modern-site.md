---
title: Výmena klasickej koreňovej lokality s modernou stránkou
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316155"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Výmena klasickej koreňovej lokality s modernou stránkou

Ak bolo vaše prostredie nastavené pred aprílom 2019, koreňovú lokalitu môžete zmeniť na modernú pomocou prostredia Microsoft PowerShell:

- Ak máte inú lokalitu, ktorú chcete použiť ako koreňovú lokalitu, môžete ju nahradiť [(vymeniť) za koreňovú](https://docs.microsoft.com/sharepoint/modern-root-site) lokalitu. 
    - Ak chcete pri archivácii pôvodnej lokality vymeniť umiestnenie lokality s inou stránkou, použite možnosť [Invoke-SPOSiteSwap.](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) K dispozícii pre tímovú lokalitu (nie je pripojená ku skupine) aj pre komunikačnú lokalitu. 

- Čoskoro sa zavedia ďalšie možnosti, ktoré vám umožnia naďalej používať obsah lokality, ale skonvertujú existujúcu lokalitu na komunikačnú lokalitu. 

**Dôležité:** Tieto možnosti sa budú zavádzať postupne. Pokračujte v kontrole aktualizácií v Centre správ. 

## <a name="known-issues-with-swapping-sites"></a>Známe problémy s výmenou lokalít

- Cieľová lokalita môže na krátky čas vrátiť chybu "nenašiel sa" (HTTP 404).
- Ak chcete aktualizovať index vyhľadávania, obsah sa bude musieť opätovne uchýliť. Nevyžaduje sa žiadny manuálny krok – táto postup sa vykonáva automaticky.
- Všetko závislé od "statických" prepojení (napríklad synchronizácia súborov a odstránenie OneNote súborov) bude potrebné manuálne opraviť.
- Ak zdrojová lokalita bola lokalitu správ organizácie, aktualizujte URL adresu. Získajte zoznam všetkých lokalít správ organizácie.
- Project Na to, aby sa aj naďalej pridruželi správne, možno bude potrebné overiť lokality servera.
