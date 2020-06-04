---
title: Aktualizácia DNS záznamov, aby sa vaša webová lokalita udržala u aktuálneho poskytovateľa hostiteľských služieb
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665775"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizácia DNS záznamov, aby sa vaša webová lokalita udržala u aktuálneho poskytovateľa hostiteľských služieb

1. V Centre spravovania služby Microsoft 365 prejdite na stránku **Setup**  >  [Domains (Nastavenia domén)](https://portal.office.com/adminportal/home#/Domains) a v zozname domén vyberte doménu, ktorú používate pre svoju webovú lokalitu.

2. Vyberte **položku + Nový vlastný záznam** a zadajte nasledujúce položky:

  - Pre **typ DNS** zadajte: A **(Adresa)**

  - Pre **názov hostiteľa alebo alias**, zadajte nasledovné:**@**

  - V prípade **adresy IP**zadajte statickú adresu IP webovej lokality, na ktorej je aktuálne hosťovaná (napríklad 172.16.140.1).

    Musí to byť *statická* adresa IP pre webovú lokalitu, nie *dynamická* adresa IP. Informujte sa u stránok, kde je vaša webová stránka hosťovaná, aby sa ubezpečil, môžete získať statickú IP adresu pre vaše verejné webové stránky.

3. Vyberte polo **ku Ulo3/4i»**.

Okrem toho môžete vytvoriť CNAME záznam, ktorý pomôže zákazníkom nájsť vaše webové stránky.
  
1. Vyberte **položku + Nový vlastný záznam** a zadajte nasledujúce položky:

  - Pre **typ DNS** zadajte: **CNAME (Alias)**

  - Pre **názov hostiteľa alebo Alias**zadajte nasledujúce: **www**

  - Ak **chcete použiť položku Smerovanie na adresu,** zadajte úplný názov domény (FQDN) pre vašu webovú lokalitu (napríklad contoso.com).

2. Vyberte polo **ku Ulo3/4i»**.
