---
title: Aktualizácia záznamov DNS na ponechaie webovej lokality u aktuálneho poskytovateľa hostiteľských služieb
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007697"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizácia záznamov DNS na ponechaie webovej lokality u aktuálneho poskytovateľa hostiteľských služieb

1. V Centrum spravovania služby Microsoft 365 prejdite na stránku **Setup** Domains (Nastavenie domén) a v zozname domén vyberte doménu, ktorú používate  >  [](https://admin.microsoft.com/Adminportal#/Domains) pre svoju webovú lokalitu.

2. Vyberte **položku + Nový vlastný záznam** a zadajte nasledovné položky:

  - Pre **typ DNS** zadajte: A **(Adresa)**

  - Do **poľa Názov hostiteľa alebo alias** zadajte nasledujúci reťazec: **@**

  - V **časti Adresa IP** zadajte statickú IP adresu svojej webovej lokality, na ktorej je momentálne hosťovaná (napríklad 172.16.140.1).

    Musí to byť  *statická*  IP adresa webovej lokality, nie  *dynamická*  IP adresa. Overte lokalitu, na ktorej je hosťovaná vaša webová lokalita, a uistite sa, že môžete získať statickú IP adresu pre svoju verejnú webovú lokalitu.

3. Vyberte **položku Uložiť**.

Okrem toho môžete vytvoriť záznam CNAME, ktorý zákazníkom pomôže nájsť vašu webovú lokalitu.
  
1. Vyberte **položku + Nový vlastný záznam** a zadajte nasledovné položky:

  - Pre **položku Typ DNS** zadajte: **CNAME (Alias)**

  - Do **poľa Názov hostiteľa alebo alias** zadajte: **www**

  - Do **poľa Points to address**(Body na adresu) zadajte plne kvalifikovaný názov domény (FQDN) svojej webovej lokality (napríklad contoso.com).

2. Vyberte **položku Uložiť**.
