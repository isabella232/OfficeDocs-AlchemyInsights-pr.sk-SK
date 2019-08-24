---
title: Read-Only na údržbu správy pri pokuse o použitie SharePoint alebo OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620738"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only na údržbu správy pri pokuse o použitie SharePoint alebo OneDrive

Používatelia môžu hlásenie **Read-Only pre údržbu** pri pokuse o použitie SharePoint alebo OneDrive pre jeden z týchto scenárov. 

-   Plánované alebo aktívna údržba činnosť.  Skontrolovať ich prechodom do [Centra správ](https://portal.office.com/adminportal/home#/messagecenter).
-   Vysokou prioritou, aktívne servisné udalosti, ktorá môže vyskytnúť. Kontrola každej návestí podpory incidentov, prechodom do [Služby zdravia](https://portal.office.com/adminportal/home#/servicehealth).
-   Drobné automatické liečenie zotavenie scenár, ktorý mohol deje z dôvodu neočakávaných udalostí na serveroch, ktoré môže trvať menej ako 30 minút alebo tak. 
    
    Neexistujú žiadne Message Center alebo služby zdravia príspevky pre tieto menšie extrakcia, ale mali by ste byť späť do normálneho veľmi skoro.

Veľmi málo príležitostiach sme pozorovali, že jeden z troch scenárov uvedených vyššie boli príčinou, a služba bola obnovená, ale cache prehliadača užívateľov nemá očistili.

Prosím pokúsi zmazať cache prehliadača pred vyhľadania lokality.

1. V prehliadači Microsoft Edge, vyberte **nastavenia**a potom vyberte položku **súkromie a bezpečnosť**.
2. Podľa **jasných prehliadania**, vyberte položku **vybrať položky na vymazanie**.
3. Vyberte **súbory cookie a uložené údaje webových lokalít**a vyberte **Vymazať**.

>[!Note] 
> Tieto kroky sa môžu líšiť, pri použití iných prehliadačov, ako Mozilla Firefox alebo Google Chrome.

>[!Note] 
> Ďalšou možnosťou by bolo otvoriť lokalitu SharePoint alebo OneDrive v nové okno v režime InPrivate.