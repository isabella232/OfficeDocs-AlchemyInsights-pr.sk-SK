---
title: Swap vaše klasickej koreňovej lokality s moderný web
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
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246071"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap vaše klasickej koreňovej lokality s moderný web

Ak vaše prostredie bola zriadená pred máj 2019, môžete zmeniť koreňovou lokalitou na moderné stránky pomocou Microsoft PowerShell:

- Ak máte rôzne stránky, ktoré chcete použiť ako koreňovú lokalitu, môžete nahradiť (swap) koreň mieste s ním. 
    - Pomocou [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie lokality s ďalším mieste počas archivácie pôvodnej lokality. K dispozícii pre tím stránky (nie je pripojený k skupine) a komunikácie miesto. 

- Ďalšie možnosti budú zavedené čoskoro ktoré vám umožní používať obsah na webe, ale prevod existujúcej lokality na lokalitu komunikácie. 
>[!Important]
>Tieto schopnosti bude postupne váľa. Pokračovať v kontrole stredisku správ v Office 365 aktualizácie. 

## <a name="known-issues-with-swapping-sites"></a>Známe problémy s vymieňania lokalít

- Cieľová lokalita môže vrátiť "nebol nájdený" chyba (HTTP 404) za krátky čas.
- Obsah bude musieť byť recrawled aktualizovať index vyhľadávania. Neexistuje žiadny manuál krok potrebný - to sa deje automaticky.
- Všetko závisí od "statické" odkazy (napríklad synchronizáciu súborov a OneNote súbory) treba manuálne opraviť.
- Ak zdroj stránky bolo organizačné Novinky stránok, aktualizácia URL.Získajte zoznam všetkých organizačných spravodajských webov.
- Project Server lokality musí validovať zabezpečiť, že sú stále spojené správne.





