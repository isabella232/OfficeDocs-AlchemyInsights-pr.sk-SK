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
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e0dadba1e3ffd1cf0d49c0a76ec2efbbc6ae92db
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906135"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualizácie záznamov DNS, aby vaše webové stránky s aktuálne poskytovateľa hostingu

1. Na stránke [domény](https://portal.office.com/adminportal/home#/Domains) v zozname domény vyberte doménu používate pre vaše webové stránky, a potom vyberte **nastavenia DNS** na table Správa. 
    
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
    

