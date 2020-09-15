---
title: Swap klasickej koreňovej lokality na modernú lokalitu
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691194"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap klasickej koreňovej lokality na modernú lokalitu

Ak bolo vaše prostredie nastavené pred aprílom 2019, koreňovú lokalitu môžete zmeniť na modernú lokalitu pomocou prostredia Microsoft PowerShell:

- Ak máte inú lokalitu, ktorú chcete použiť ako koreňovú lokalitu, môžete ju nahradiť [(vymeniť) koreňovú lokalitu](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Pri archivácii pôvodnej lokality môžete použiť [vyvolanie-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) na výmenu umiestnenia lokality s inou lokalitou. K dispozícii pre tímovú lokalitu (nie je pripojená k skupine) a na komunikačnú lokalitu. 

- Čoskoro sa dodajú ďalšie možnosti, ktoré vám umožnia naďalej používať obsah lokality, ale skonvertovať existujúcu lokalitu na komunikačnú lokalitu. 
>[!Important]
>Tieto možnosti sa budú postupne zavádzať. Pokračujte v kontrole aktualizácií v centre správ. 

## <a name="known-issues-with-swapping-sites"></a>Známe problémy pri výmene lokalít

- Cieľová lokalita môže počas krátkeho časového obdobia vrátiť chybu not found (HTTP 404).
- Ak chcete aktualizovať index vyhľadávania, bude potrebné prehľadať obsah. Nevyžaduje sa žiadny manuálny krok – tento postup sa vykoná automaticky.
- Všetko, čo je závislé od statických prepojení (ako je napríklad synchronizácia súborov a OneNote), bude potrebné manuálne opraviť.
- Ak je zdrojovou lokalitou lokalita na správu organizácie, aktualizujte URL adresu.Získajte zoznam všetkých lokalít organizačných správ.
- Lokality programu Project Server možno bude potrebné overiť, aby sa zabezpečilo, že sú stále priradení správne.
