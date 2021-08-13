---
title: Obmedziť SharePoint online na klasický režim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958816"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Obmedziť SharePoint online na klasický režim

Niektoré organizácie stále vyžadujú klasický režim. Hoci na podrobnej úrovni neexistujú žiadne plány na odstránenie klasického režimu, nie je možné obmedziť režim celej organizácie (nájomníka) na klasický režim pre zoznamy a knižnice.

Správca bude mať k dispozícii nasledujúce možnosti na spravovanie jednotlivých zoznamov a knižníc v klasickom režime pomocou granulárneho prepínača explicitných nesúhlasov, ktoré poskytujeme na nasledujúcich úrovniach:

- kolekcia lokalít
- lokalita
- zoznam
- knižnica

Zoznamy, ktoré používajú niektoré funkcie a prispôsobenia, ktoré nie sú podporované modernými zariadeniami, sa navyše automaticky prepnú na klasický režim.

Od 1. apríla 2019 sa proces vypnutia moderného zoznamu a knižníc na úrovni nájomníka začne a bude pokračovať až do 31. mája 2019.  Zoznamy a knižnice, ktoré sú v klasickom režime ako výsledok odhlásenie nájomníka, sa automaticky presunú do moderného režimu.

Ak potrebujete klasický režim, [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) pozrite si ďalšie informácie [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) tu a pokyny pre prostredie PowerShell pre PnP tu popisujú možnosti a nástroje, ktoré môžete v súčasnosti použiť na používanie klasického režimu.
