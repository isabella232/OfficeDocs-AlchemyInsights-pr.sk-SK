---
title: Swap klasickej koreňovej stránky s moderným mieste
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749275"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap klasickej koreňovej stránky s moderným mieste

Ak bolo vaše prostredie nastavené pred aprílom 2019, môžete zmeniť koreňovú lokalitu na modernú lokalitu pomocou prostredia Microsoft PowerShell:

- Ak máte inú lokalitu, ktorú chcete použiť ako svoju koreňovú lokalitu, môžete s ňou nahradiť [(vymeniť) koreňovú lokalitu](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Použitie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie stránky s inou lokalitou pri archivácii pôvodnej stránky. K dispozícii pre obe tímové stránky (nie je pripojený k skupine) a komunikačné stránky. 

- Ďalšie možnosti budú predstavené čoskoro, že vám umožní udržať používanie obsahu na webe, ale previesť existujúce stránky na komunikačné miesto. 
>[!Important]
>Tieto schopnosti budú postupne váľa. Pokračovať v kontrole Office 365 centrum správ pre aktualizácie. 

## <a name="known-issues-with-swapping-sites"></a>Známe problémy s vymenením lokalít

- Cieľová lokalita môže vrátiť chybu "Not Found" (HTTP 404) na krátku dobu.
- Obsah bude musieť byť recrawled aktualizovať vyhľadávací index. Nie je potrebný manuálny krok-to bude vykonané automaticky.
- Čokoľvek závislé na "statické" odkazy (napríklad synchronizácia súborov a súbory programu OneNote) bude potrebné manuálne opraviť.
- Ak zdrojová lokalita bola lokalita správy organizácie, aktualizujte adresu URL.Získajte zoznam všetkých organizačných spravodajských webov.
- Lokality Project Server môže byť potrebné overiť, aby sa zabezpečilo, že sú stále spojené správne.





