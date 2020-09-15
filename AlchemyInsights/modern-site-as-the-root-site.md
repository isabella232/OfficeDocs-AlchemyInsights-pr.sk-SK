---
title: Moderná lokalita ako Koreňová lokalita
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666885"
---
# <a name="modern-site-as-root-site"></a>Moderná lokalita ako Koreňová lokalita

Začali sme zavádzať novú funkciu, ktorá vám umožní [vymieňať si klasickú koreňovú lokalitu lokality s modernou lokalitou](https://docs.microsoft.com/sharepoint/modern-root-site). Pri archivácii pôvodnej lokality môžete použiť [vyvolanie-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) na výmenu umiestnenia lokality s inou lokalitou. K dispozícii pre tímovú lokalitu (nie je pripojená k skupine) a na komunikačnú lokalitu.

>[!Important]
> Neodstraňujte klasickú koreňovú lokalitu a vytvorte modernú komunikačnú lokalitu. Spoločnosť Microsoft to nepodporuje. Odstránením koreňovej lokality budú všetky lokality SharePoint vo vašej organizácii neprístupné pre všetkých používateľov, kým neobnovíte lokalitu alebo nevytvoríte novú lokalitu na rovnakej URL adrese. Túto funkciu budeme komunikovať prostredníctvom centra správ. V najbližšej dobe by ste mali očakávať, že funkcia bude v nájomníkovi zapnutá.

## <a name="known-issues-with-swapping-sites"></a>Známe problémy pri výmene lokalít
- Cieľová lokalita môže počas krátkeho časového obdobia vrátiť chybu not found (HTTP 404).
- Ak chcete aktualizovať index vyhľadávania, bude potrebné prehľadať obsah. Tu nie je potrebný manuálny krok, tento postup sa vykoná automaticky.
- Všetko, čo je závislé od statických prepojení (ako je napríklad synchronizácia súborov a OneNote), bude potrebné manuálne opraviť.
- Lokality programu Project Server možno bude potrebné overiť, aby sa zabezpečilo, že sú stále priradení správne. 
