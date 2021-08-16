---
title: Zisťovanie lokalít
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030773"
---
# <a name="do-site-discovery"></a>Zisťovanie lokalít

Ak vaša organizácia stále používa staršie webové aplikácie a plánuje používať režim Internet Explorera (čo väčšina zákazníkov má), mali by ste urobiť niekoľko ďalších zisťovaní lokalít.

**Už ste nasadili staršiu verziu Microsoft Edge**

Ak ste už nakonfigurovali zoznam podnikových lokalít na prácu so staršou verziou balíka Microsoft Edge, zisťovanie lokality je už takmer hotové. Možno budete musieť urobiť len pridanie neutrálnych lokalít.

Neutrálne lokality sú zvyčajne lokality, ktoré poskytujú jediné prihlásenie. Ak prejdete na neutrálnu lokalitu z Microsoft Edge, potom chcete zostať pri Microsoft Edge overiť. Ak prejdete na neutrálnu lokalitu v režime Internet Explorera, potom chcete zostať v režime Internet Explorera a overiť ich.

Identifikujte všetky neutrálne lokality alebo lokality, ktoré používate, a pridajte ich do zoznamu podnikových lokalít.

**Predvolený prehliadač je Internet Explorer**

Ak teraz používate Iba Internet Explorer, možno neviete, ktoré lokality sú inovované na moderné webové štandardy a ktoré stále vyžadujú Internet Explorer. Tieto lokality budete chcieť vyhľadať a pridať do zoznamu podnikových lokalít, aby ste mohli používať režim Internet Explorera iba pre tieto lokality.

> [!NOTE]
> [Podnikové zisťovanie](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) lokalít vyhľadáva lokality, ktoré by mohli potrebovať režim Internet Explorera. Môže zhromažďovať údaje v počítačoch s Windows Internet Explorerom 8 prostredníctvom Internet Explorera 11 v Windows 10, Windows 8.1 alebo Windows 7.

**Analýza údajov**

Po zozbieraní údajov lokality odporúčame na analýzu údajov vykonať tieto štyri kroky:
1. Zoraďte údaje podľa domény a potom podľa URL adresy.
2. Definujte hranice aplikácie, ktoré sa majú konfigurovať pre režim Internet Explorera. Chcete zahrnúť všetky lokality a webové ovládacie prvky, ktoré definujú aplikáciu, ale nechcete do nich zahrnúť ďalšie lokality a ovládacie prvky. Niektoré lokality môžu byť rovnako jednoduché, *https://contoso.com/app1* zatiaľ čo iné môžu vyžadovať definovanie viacerých lokalít a stránok.
3. Otestujte aplikáciu a overte, či nefunguje natívne. Mnohé lokality budú ponúkať moderný obsah, keď zistia moderný prehliadač a ponúknu starší obsah len vtedy, keď zistia Internet Explorer.
4. Ak aplikácia zlyhá, pridajte ju do zoznamu podnikových lokalít.

> [!NOTE]
> Najlepšie je zoskupiť všetky lokality, ktoré tvoria aplikáciu. Týmto spôsobom je pri inovácii aplikácie jednoduchšie odstrániť celú lokalitu z režimu Internet Explorera a začať používať moderný prehliadač pre túto aplikáciu.

Po zistení lokality a analýze údajov môžete začať s analýze stratégie kanála.

