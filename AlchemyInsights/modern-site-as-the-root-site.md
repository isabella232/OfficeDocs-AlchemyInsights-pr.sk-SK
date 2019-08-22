---
title: Moderné lokalitu ako root
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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543868"
---
# <a name="modern-site-as-root-site"></a>Moderné lokalitu ako root

My sme začali rollout novú funkciu, ktorá vám umožní vymeniť lokality klasické miesto koreňové s moderný web. Pomocou [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) swap umiestnenie lokality s ďalším mieste počas archivácie pôvodnej lokality. K dispozícii pre tím stránky (nie je pripojený k skupine) a komunikácie miesto. 

>[!Important]
> Neodstraňujte klasickej koreňovej lokality vytvoriť lokalitu modernej komunikácie. To nie je podporovaný spoločnosťou Microsoft. Odstránenie koreňovej lokality bude všetkých lokalít SharePoint vo vašej organizácii neprístupné pre všetkých užívateľov, kým obnovenie lokality alebo vytvoriť novú lokalitu na rovnakú adresu URL. Sme bude komunikovať Táto funkcia cez centra správ. By ste očakávať funkcie musia byť zapnuté v nájomcu krátko.

## <a name="known-issues-with-swapping-sites"></a>Známe problémy s vymieňania lokalít
- Cieľová lokalita môže vrátiť "nebol nájdený" chyba (HTTP 404) za krátky čas.
- Obsah bude musieť byť recrawled aktualizovať index vyhľadávania. Neexistuje žiadny manuál krok vyžaduje tu, to sa deje automaticky.
- Všetko závisí od "statické" odkazy (napríklad synchronizáciu súborov a OneNote súbory) treba manuálne opraviť.
- Project Server lokality musí validovať zabezpečiť, že sú stále spojené správne. 
