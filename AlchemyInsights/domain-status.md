---
title: Domain Status - No services selected
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1ddf6475e7cf466a39f76486e0f809097917657bc8f4ae7f7f2b516657308f39
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947458"
---
# <a name="domain-status---no-services-selected"></a>Domain Status - No services selected

**Výber žiadnych** služieb znamená, že ste pre služby Microsoft 365 ako Exchange Online, Skype for Business alebo Intune a Správa mobilných zariadení pre Microsoft 365 nevyznali žiadne služby, ktoré by ste mali používať s vlastnou doménou. Ak používate hybridné Exchange (Exchange lokálne so systémom Exchange Online) alebo externé filtrovanie nevyžiadanej pošty pomocou Exchange a žiadne iné služby Microsoft, môžete toto hlásenie ignorovať. Stav domény je k dispozícii iba pre domény pripojené priamo k službe.

Výber služieb pre doménu:

1. V **Nastavenia**  >  [**Domains (Domény)**](https://admin.microsoft.com/Adminportal/Home)začiarknite políčko vedľa domény so správou o stave **Žiadne služby (bez vybratých služieb).**
1. Výberom **položky Manage DNS (Spravovať DNS)** spustite Sprievodcu nastavením domény.
    - Ak vyberiete **položku Add your own DNS records**(Pridať vlastné DNS záznamy), po zobrazení výzvy vyberte službu. Ďalšie služby môžu byť k dispozícii v **časti Rozšírené možnosti.**
    - Ak vyberiete **možnosť Dovoľte spoločnosti Microsoft pridať vaše DNS** záznamy alebo **Ďalšie** možnosti Nastaviť moje online služby pre mňa všetky dostupné služby sa budú  >   navrhovať a vyberať automaticky.
1. Pokračujte v sprievodcovi a dokončite nastavenie DNS systému a výber služieb.
 
Ďalšiu pomoc s nastavením domény nájdete v téme [Pridanie DNS záznamov na pripojenie domény.](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

