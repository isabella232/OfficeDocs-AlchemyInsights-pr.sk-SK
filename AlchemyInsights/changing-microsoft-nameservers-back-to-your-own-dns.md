---
title: Zmena z názvových serverov spoločnosti Microsoft späť na spravovanie vlastných DNS záznamov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506972"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Zmena z názvových serverov spoločnosti Microsoft späť na spravovanie vlastných DNS záznamov

Predtým ste zmenili svoje NS záznamy tak, aby ukazovali na spoločnosť Microsoft (ns1.bdm.microsoftonline.com), ale teraz ste sa rozhodli spravovať vlastné DNS záznamy:

Na webovej lokalite registrátora domén zmeňte názvový server späť na svojho registrátora alebo predchádzajúce nastavenie. Ak nemáte dns systém známy, obráťte sa na oddelenie technickej podpory registrátora domén. Všimnite si, že rozšírenie zmien názvových serverov môže trvať až 48 hodín. 

1. Na portáli Microsoft 365 prejdite na **položku Nastavenia** Domains (Domény) , začiarknite políčko vedľa domény a  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)vyberte položku Manage **DNS (Spravovať DNS).** 

2. V sprievodcovi vyberte položku **Pridať vlastné DNS záznamy a** dokončite sprievodcu. Zmení sa spôsob správy DNS systému a potom môžete pridať vlastné DNS záznamy potrebné na podporu vybratých služieb.

Prípadne ak ste zmenili záznamy názvového servera na spoločnosť Microsoft a máte webovú lokalitu, môžete pridať DNS záznamy webovej lokality namiesto toho, aby ste názvové servery zmenili späť. Ďalšie informácie nájdete v téme Aktualizácia [záznamov DNS na ponechaie webovej lokality u aktuálneho poskytovateľa hostiteľských služieb.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


