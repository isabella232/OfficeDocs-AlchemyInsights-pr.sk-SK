---
title: Iba na čítanie pre správu údržby pri pokuse o použitie SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051296"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Iba na čítanie pre správu údržby pri pokuse o použitie SharePoint alebo OneDrive

Používatelia môžu zobraziť **iba na čítanie pre údržbu** správy pri pokuse o použitie SharePoint alebo OneDrive pre jeden z nasledujúcich scenárov. 

-   Plánovanej alebo aktívnej činnosti údržby.  Vyhľadajte ich tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/messagecenter).
-   Vysoká priorita, aktívny servisný incident, ktorý môže byť vyskytujúci sa. Vyhľadajte všetky upozornenia/incidenty tým, že prejdete na [stav služby](https://portal.office.com/adminportal/home#/servicehealth).
-   Menšie auto-liečenie zotavenie scenár, ktorý by mohol byť deje v dôsledku neočakávaných udalostí na serveroch, ktoré by mohli trvať menej ako 30 min alebo tak. 
    
    Neexistujú žiadne správy centra alebo služby zdravia miest pre tieto drobné vymáhanie, ale mali by ste byť späť do normálu veľmi skoro.

Na veľmi málo príležitostiach sme pozorovali, že jeden z troch scenárov uvedených vyššie boli príčinou, a služba bola obnovená, ale užívatelia prehliadač cache nebol vymazaný.

Pred navigáciou na lokalitu sa pokúste vymazať vyrovnávaciu pamäť prehľadávača.

1. V prehľadávači Microsoft Edge vyberte položku **Nastavenie**a potom vyberte položku **Ochrana osobných údajov a zabezpečenie**.
2. V časti **Vymazanie prehľadávania**vyberte položku **vybrať, čo sa má vymazať**.
3. Vyberte položku **súbory cookie a uložené údaje webových stránok**a vyberte položku **Vymazať**.

>[!Note] 
> Tieto kroky sa môžu líšiť pri používaní iných prehliadačov, ako je Mozilla Firefox alebo Google Chrome.

>[!Note] 
> Ďalšou možnosťou by bolo otvoriť lokalitu SharePoint alebo OneDrive v novom okne v režime InPrivate.