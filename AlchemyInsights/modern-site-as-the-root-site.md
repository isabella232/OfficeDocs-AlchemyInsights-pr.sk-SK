---
title: Moderné stránky ako koreňovej stránky
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753919"
---
# <a name="modern-site-as-root-site"></a>Moderné stránky ako root site

Začali sme zavádzanie novej funkcie, ktorá vám umožní [vymeniť klasické stránky koreňovej stránky s moderným mieste](https://docs.microsoft.com/sharepoint/modern-root-site). Použitie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie stránky s inou lokalitou pri archivácii pôvodnej stránky. K dispozícii pre obe tímové stránky (nie je pripojený k skupine) a komunikačné stránky.

>[!Important]
> Neodstraňujte svoju klasickú koreňovú stránku na vytvorenie modernej komunikačnej stránky. Toto nie je podporovaný spoločnosťou Microsoft. Odstránením koreňovej lokality sa všetky lokality SharePoint vo vašej organizácii neprístupné všetkým používateľom, kým neobnovíte lokalitu alebo vytvoríte novú lokalitu na rovnakej adrese URL. Túto funkciu budeme komunikovať prostredníctvom centra správ. Mali by ste očakávať, že funkcia bude zapnutá v nájomcovi krátko.

## <a name="known-issues-with-swapping-sites"></a>Známe problémy s vymenením lokalít
- Cieľová lokalita môže vrátiť chybu "Not Found" (HTTP 404) na krátku dobu.
- Obsah bude musieť byť recrawled aktualizovať vyhľadávací index. Neexistuje žiadny manuálny krok vyžaduje tu, to bude vykonané automaticky.
- Čokoľvek závislé na "statické" odkazy (napríklad synchronizácia súborov a súbory programu OneNote) bude potrebné manuálne opraviť.
- Lokality Project Server môže byť potrebné overiť, aby sa zabezpečilo, že sú stále spojené správne. 
