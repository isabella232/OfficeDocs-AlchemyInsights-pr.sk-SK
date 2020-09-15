---
title: Iba na čítanie správy o údržbe pri pokuse o používanie SharePointu alebo OneDrivu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670847"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Iba na čítanie správy o údržbe pri pokuse o používanie SharePointu alebo OneDrivu

Pri pokuse o používanie SharePointu alebo OneDrivu pre niektorý z nasledujúcich scenárov môžu používatelia dostávať správu o **údržbe iba na čítanie** . 

-   Plánovaná alebo aktívna aktivita údržby.  Vyhľadajte ich tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/messagecenter).
-   Aktívny incident služby s vysokou prioritou, ktorý sa môže vyskytnúť. Vyhľadajte všetky upozornenia alebo incidenty navigáciou na [stav služby](https://portal.office.com/adminportal/home#/servicehealth).
-   Malý scenár obnovenia automatického hojenia, ktorý by sa mohol stať v dôsledku neočakávaných udalostí na serveroch, ktoré môžu trvať menej ako 30 minút alebo tak. 
    
    Nie sú k dispozícii žiadne centrá správ ani príspevky týkajúce sa zdravotníckych služieb pre tieto drobné zotavuje, ale mali by ste sa vrátiť k normálu veľmi skoro.

Pri veľmi málo príležitostiach sme zistili, že jedným z týchto troch scenárov boli príčiny a služba bola obnovená, ale vyrovnávacia pamäť prehliadača používateľov nebola vymazaná.

Skôr než prejdete na lokalitu, skúste vymazať vyrovnávaciu pamäť prehliadača.

1. V prehliadači Microsoft Edge vyberte položku **Nastavenie**a potom vyberte položku **Ochrana osobných údajov a zabezpečenie**.
2. V časti **Vymazanie prehľadávania**vyberte položku **vybrať položky, ktoré chcete vymazať**.
3. Vyberte položku **súbory cookie a uložené údaje webovej lokality**a vyberte položku **Vymazať**.

>[!Note] 
> Tieto kroky sa môžu líšiť pri používaní iných prehliadačov, ako je napríklad Mozilla Firefox alebo Google Chrome.

>[!Note] 
> Ďalšou možnosťou by bolo otvoriť lokalitu SharePoint alebo OneDrive v novom okne v režime InPrivate.