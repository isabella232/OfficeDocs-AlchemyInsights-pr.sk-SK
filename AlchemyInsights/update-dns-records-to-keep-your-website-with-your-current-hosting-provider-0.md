---
title: Aktualizujte DNS záznamy, aby ste mali webovú lokalitu so súčasným poskytovateľom hostiteľských služieb.
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815800"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizujte DNS záznamy, aby ste mali webovú lokalitu so súčasným poskytovateľom hostiteľských služieb.

1. V centre spravovania služby Microsoft 365 prejdite na stránku **Nastavenie**  >  [domén](https://admin.microsoft.com/Adminportal#/Domains) a v zozname domén vyberte doménu, ktorú používate pre svoju webovú lokalitu.

2. Vyberte položku **+ nový vlastný záznam** a zadajte tieto možnosti:

  - **Typ DNS** zadajte: **A (adresa)**

  - Pre **názov hostiteľa alebo alias**zadajte nasledovné: **@**

  - Pre **adresu IP**zadajte statickú IP adresu svojej webovej lokality, na ktorej je v súčasnosti hosťovaná (napríklad 172.16.140.1).

    Musí to byť  *statická*  IP adresa webovej lokality, nie  *dynamická*  IP adresa. Skontrolujte, či je lokalita, na ktorej je vaša webová lokalita hosťovaná, a uistite sa, že môžete získať statickú IP adresu svojej verejnej webovej lokality.

3. Vyberte položku **Uložiť**.

Okrem toho môžete vytvoriť CNAME záznam, ktorý zákazníkom pomôže nájsť vašu webovú lokalitu.
  
1. Vyberte položku **+ nový vlastný záznam** a zadajte tieto možnosti:

  - **Typ DNS** zadajte: **CNAME (alias)**

  - Ak máte **názov hostiteľa alebo alias**, zadajte: **www**

  - V prípade **bodov na adresu**Zadajte úplný názov domény (FQDN) svojej webovej lokality (napríklad contoso.com).

2. Vyberte položku **Uložiť**.
