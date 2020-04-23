---
title: Swap klasickej koreňovej stránky s moderným mieste
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741559"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap klasickej koreňovej stránky s moderným mieste

Ak bolo vaše prostredie nastavené pred aprílom 2019, môžete zmeniť koreňovú lokalitu na modernú lokalitu pomocou prostredia Microsoft PowerShell:

- Ak máte inú lokalitu, ktorú chcete použiť ako svoju koreňovú lokalitu, môžete s ňou nahradiť [(vymeniť) koreňovú lokalitu](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Použitie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie stránky s inou lokalitou pri archivácii pôvodnej stránky. K dispozícii pre obe tímové stránky (nie je pripojený k skupine) a komunikačné stránky. 

- Ďalšie možnosti budú predstavené čoskoro, že vám umožní udržať používanie obsahu na webe, ale previesť existujúce stránky na komunikačné miesto. 
>[!Important]
>Tieto schopnosti budú postupne váľa. Pokračujte v kontrole aktualizácií centra správ. 

## <a name="known-issues-with-swapping-sites"></a>Známe problémy s vymenením lokalít

- Cieľová lokalita môže vrátiť chybu "Not Found" (HTTP 404) na krátku dobu.
- Obsah bude musieť byť recrawled aktualizovať vyhľadávací index. Nie je potrebný manuálny krok-to bude vykonané automaticky.
- Čokoľvek závislé na "statické" odkazy (napríklad synchronizácia súborov a súbory programu OneNote) bude potrebné manuálne opraviť.
- Ak zdrojová lokalita bola lokalita správy organizácie, aktualizujte adresu URL.Získajte zoznam všetkých organizačných spravodajských webov.
- Lokality Project Server môže byť potrebné overiť, aby sa zabezpečilo, že sú stále spojené správne.
