---
title: Problém s filtrom atribútu a rozsahu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482921"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problém s filtrom atribútu a rozsahu

**Problém s kolidujúcimi hodnotami hlavného mena používateľa**

Pracovný deň na poskytovanie AD User (pracovný deň) na poskytovanie AD používateľov zobrazuje chybové hlásenie **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Operácia zlyhala, pretože hodnota hlavného mena používateľa poskytnutá na sčítanie alebo úpravu nie je jedinečná. Podrobnosti o chybe: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

Hodnota **userPrincipalName** , ktorá sa pri vytváraní používateľského konta v reklame, ktorá sa pokúša nastaviť, sa v doméne cieľová reklama už vyskytuje. To znamená, že buď (1) používateľ už existuje, a kontrola zhodných IDENTIFIKÁCIí pre používateľa zlyhala alebo (2) pravidlo generácie UPN vygenerovalo kolidujúcu hodnotu.

Tu sú navrhované kroky riešenia:

Ak už používateľ existuje a kontrola TOTOŽNosti sa nepodarilo prepojiť konto pracovného dňa s kontom služby Active Directory, skontrolujte, či sa zhoda s atribútom ID (zvyčajne **klíč**) v oboch pracovný deň aj v reklame presne zhoduje. Ak sa nezhodujú, ide o problém s údajmi, ktorý treba opraviť. Ak je napríklad identifikácia zamestnanca v pracovnom hárku 001052 a v REKLAMe je 1052, potom sa pri zriaďovaní motora nepodarí prepojiť dva kontá a pokúsiť sa vytvoriť používateľa, ktorý už existuje. Riešenie v tomto prípade je zmeniť hodnotu **klíč** v reklame tak, aby obsahovala úvodné nuly, aby bolo 001052.
Ak výraz generovanie UPN nevytvára jedinečnú hodnotu, zvážte použitie funkcie de-duplikácie **SelectUniqueValue** na vytvorenie jedinečnej hodnoty pri každom spustení.

**Pracovný deň na poskytovanie AD User nenastaví hodnotu atribútu Manager pre konto AD User**

V pracovnom postupe AD User na poskytovanie úloh sa nenastaví hodnota atribútu **Manager** pre kontá ad user. Ak sa toto správanie zobrazuje, existujú dva možné scenáre:

1. Manažér v pracovný deň nie je možné preložiť na zodpovedajúce konto AD User, pretože manažér nie je v rozsahu.
2. V scenári s **viacerými reklamnými doménami** sa manažér v pracovný deň nenachádza v rovnakej doméne ako používateľ.

Skúste problém vyriešiť pomocou týchto krokov:

1. Ak ste definovali rozsahy filtrov, najskôr skontrolujte, či je manažér v rozsahu a či spĺňa klauzulu rozsahov. Ak manažér nevyhovuje filtru rozsahu, zmeňte filter tak, aby bol manažér v rozsahu operácie poskytovania.
2. Ak máte viacero REKLAMných domén, konektor má známe obmedzenie nemožnosti riešenia odkazov na krížový správca domény.

Ďalšie informácie o konfigurácii pracovného dňa na automatické poskytovanie informácií nájdete v téme [kurz: Konfigurácia pracovného dňa na automatické poskytovanie používateľov](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













