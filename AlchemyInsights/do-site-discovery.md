---
title: Zisťovanie lokality
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694558"
---
# <a name="do-site-discovery"></a>Zisťovanie lokality

Ak vaša organizácia stále používa staršie webové aplikácie a plány na používanie režimu Internet Explorer (ktoré väčšina zákazníkov robí), mali by ste vykonať ďalšie vyhľadávanie lokalít.

**Už ste nasadili staršiu verziu prehliadača Microsoft Edge**

Ak ste už zoznam podnikových lokalít nakonfigurovali tak, aby fungoval pre staršiu verziu prehliadača Microsoft Edge, zisťovanie lokality je takmer hotové. Je možné, že je potrebné pridať neutrálne lokality.

Neutrálne lokality sú zvyčajne lokality, ktoré poskytujú jediné prihlásenie (SSO). Ak prejdete na neutrálne miesto v prehliadači Microsoft Edge, potom sa chcete vrátiť do prehliadača Microsoft Edge. Ak prejdete na neutrálnu lokalitu v režime Internet Explorer, v režime Internet Explorer sa chcete overiť.

Identifikujte všetky SSO alebo iné neutrálne lokality, ktoré používate, a pridajte ich do zoznamu podnikových lokalít.

**Internet Explorer je predvoleným prehliadačom**

Ak teraz používate Internet Explorer, možno neviete, ktoré lokality boli inovované na moderné webové štandardy a ktoré stále vyžadujú Internet Explorer. Tieto lokality budete chcieť nájsť a pridať do zoznamu podnikových lokalít, aby ste mohli používať režim Internet Explorera len pre tieto lokality.

> [!NOTE]
> [Zisťovanie podnikovej lokality](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) zistí lokality, ktoré môžu potrebovať režim programu Internet Explorer. Môže zhromažďovať údaje v počítačoch s Windowsom Internet Explorerom 8 cez Internet Explorer 11 vo Windowse 10, Windowse 8,1 alebo Windowse 7.

**Analýza údajov**

Po zhromaždení údajov lokality odporúčame, aby ste údaje analyzovali nasledujúcim procesom:
1. Zoraďte údaje podľa domény a potom podľa URL adresy.
2. Definujte hranice aplikácie, ktorá sa má konfigurovať v režime Internet Explorer. Chcete zahrnúť všetky lokality a webové ovládacie prvky, ktoré definujú aplikáciu, ale nechcete zahrnúť ďalšie lokality a ovládacie prvky. Niektoré lokality môžu byť jednoduché, pretože *https://contoso.com/app1* iné môžu vyžadovať definovanie viacerých lokalít a stránok.
3. Otestujte aplikáciu a overte, či nefungovala natívne. Mnoho lokalít ponúkne moderný obsah pri zisťovaní moderného prehliadača a ponúka iba starší obsah pri zisťovaní programu Internet Explorer.
4. Ak zlyhá testovanie, pridajte aplikáciu do zoznamu podnikových lokalít.

> [!NOTE]
> Ako najvhodnejší postup sa zoskupujú všetky lokality, ktoré obsahujú aplikáciu. Týmto spôsobom je pri inovácii aplikácie jednoduchšie odstrániť celú lokalitu z režimu Internet Explorer a začať používať moderný prehliadač pre danú aplikáciu.

Po dokončení vyhľadávania lokality a analyzovaní údajov môžete začať pozerať na svoju stratégiu kanála.

