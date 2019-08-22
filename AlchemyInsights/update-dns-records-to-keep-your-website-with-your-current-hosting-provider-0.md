---
title: Aktualizácie záznamov DNS, aby vaše webové stránky s aktuálne poskytovateľa hostingu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506422"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizácie záznamov DNS, aby vaše webové stránky s aktuálne poskytovateľa hostingu

1. Na stránke [domény](https://portal.office.com/adminportal/home#/Domains) v zozname domény vyberte doménu, ktorú používate pre vaše webové stránky.

2. Vyberte položku **+ nový vlastný rekord** a zadajte nasledujúce:

  - Pre **Typ DNS** zadajte: **(adresa)**

  - Pre **názov hostiteľa alebo Alias**, zadajte nasledovný príkaz:**@**

  - **Adresa IP**zadajte statickú adresu IP pre vaše webové stránky, kde je v súčasnosti hostil (napríklad 172.16.140.1).

    Musí to byť *statická* adresa IP pre webové stránky, nie *dynamickú* IP adresu. Skontrolujte s lokalitou, kde je hostiteľom vašich webových stránkach aby sa ubezpečil, môžete získať statickú adresu IP pre vaše verejné webové stránky.

3. Kliknite na tlačidlo **Uložiť**.

Okrem toho môžete vytvoriť záznam CNAME pre zákazníkov nájsť vaše webové stránky.
  
1. Vyberte položku **+ nový vlastný rekord** a zadajte nasledujúce:

  - Pre **Typ DNS** zadajte: **CNAME (Alias)**

  - Pre **názov hostiteľa alebo Alias**, zadajte nasledujúce: **www**

  - **Bodov na adresu**, zadajte plne kvalifikovaní doménové meno (FQDN) pre vaše webové stránky (napríklad contoso.com).

2. Kliknite na tlačidlo **Uložiť**.
