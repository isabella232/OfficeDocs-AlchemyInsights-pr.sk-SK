---
title: Read-Only pre údržbu pri pokuse o používanie služby SharePoint alebo OneDrive
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
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329463"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only pre údržbu pri pokuse o používanie služby SharePoint alebo OneDrive

Používatelia môžu dostať hlásenie **iba na čítanie pre** údržbu pri pokuse o SharePoint alebo OneDrive pre niektorý z nasledujúcich scenárov. 

-   Plánovaná alebo aktívna údržba.  Skontrolujte ich prechodom do [Centra správ.](https://portal.office.com/adminportal/home#/messagecenter)
-   Môže sa vyskytol incident s vysokou prioritou aktívneho servisu. Ak chcete skontrolovať všetky upozornenia alebo incidenty, prechodom na [položku Stav služby.](https://portal.office.com/adminportal/home#/servicehealth)
-   Menší scenár automatického obnovenia v spoločnosti Microsoft, ktorý by sa mohol vyskytol v dôsledku neočakávaných udalostí na serveroch, ktoré môžu trvať menej ako 30 minút. 
    
    Tieto menšie obnovenia nie sú k dispozícii žiadne príspevky v Centre správ alebo stave služby, ale v normálnom stave by ste sa mali vrátiť veľmi skoro.

Pri veľmi niekoľkých príležitostiach sme si poznamenali, že príčinou bol jeden z troch uvedených scenárov a služba sa obnovila, ale vyrovnávacia pamäť prehliadača používateľov nebola vymazaná.

Pred prechodom na lokalitu sa pokúste vymazať vyrovnávaciu pamäť prehliadača.

1. V prehliadači Microsoft Edge vyberte **položku** Nastavenia a potom vyberte položku Ochrana osobných údajov a **zabezpečenie**.
2. V **časti Vymazanie prehľadávania** vyberte **položku Vybrať položky na vymazanie**.
3. Vyberte **položku Súbory cookie a uložené údaje webovej** lokality a vyberte položku **Vymazať**.

**Poznámka:** Tieto kroky sa môžu líšiť pri používaní iných prehliadačov, ako je napríklad Mozilla Firefox alebo Google Chrome.

**Poznámka:** Ďalšou možnosťou by bolo otvorenie novej SharePoint lokality alebo OneDrive v novom okne v režime InPrivate.