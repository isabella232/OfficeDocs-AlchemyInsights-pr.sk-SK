---
title: Uviazol v priečinku Pošta na odoslanie z dôvodu veľkých príloh
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441320"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Oprava správ, ktoré sú prilepené v priečinku Pošta na odoslanie

Odporúčame vám začať spustením scenára ["Mám problémy s odosielaním, prijímaním alebo vyhľadávaním e-mailových správ"](https://aka.ms/SaRA-OutlookSendReceive) z nástroja [technickej podpory a obnovenia programu Microsoft](https://diagnostics.office.com/#/) .

Keď správa uviazne v priečinku Pošta na odoslanie, Najpravdepodobnejšie príčiny sú:
- Veľké prílohy.
- Možnosť **Odoslať okamžite po pripojení** nie je povolená.

Ak chcete odstrániť veľké prílohy: 

1. V programe Outlook vyberte položku **Odoslať a prijať** > **prácu v režime offline**. 
2. Na navigačnej table vyberte položku **Pošta na odoslanie**. Odtiaľ môžete: 
    - Odstráňte správu (vyberte ju a potom vyberte položku **Delete**).
    - Presuňte správu do priečinka Koncepty, dvojitým kliknutím ho otvorte a odstráňte ju vyberte a potom vyberte položku **Delete (odstrániť**).
3. Ak sa zobrazí chyba, ktorá hovorí, že program Outlook sa pokúša odovzdať správu, zavrite program Outlook. Ukončenie môže trvať niekoľko okamihov. Ak sa program Outlook nezavrie, stlačte kombináciu klávesov CTRL + ALT + DELETE a vyberte položku **Spustiť správcu úloh**. V Správcovi úloh vyberte kartu **procesy** , posuňte sa nadol do programu Outlook. exe a vyberte položku **ukončiť proces**.
4. Po zatvorení programu Outlook, reštartujte ho a zopakujte kroky 2 a 3. 
5. Po odstránení prílohy kliknite na položku **Odoslať a prijať** > **prácu v režime offline** a pokračujte v práci online. 

Správy tiež uviaznu v priečinku Pošta na odoslanie po kliknutí na tlačidlo **Odoslať**, ale nie ste pripojení. Kliknite na tlačidlo **Odoslať a prijať** a pozrite sa na tlačidlo **pracovať v režime offline** . Ak je modrá, ste odpojený. Vyberte ho pre pripojenie (tlačidlo sa zmení na bielu) a kliknite na tlačidlo **Odoslať všetko**.
 
Ak chcete povoliť **odosielanie ihneď po pripojení**:
 
- Vyberte **** > **** možnosti >  súboru**Rozšírené**.
V časti **Odoslať a prijať** vyberte položku **Odoslať ihneď po pripojení**a potom kliknite na **tlačidlo OK**.
 
Podrobné informácie nájdete na:
- [Video: odoslanie alebo odstránenie uviaznutia e-mailu](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-mail zostane v priečinku Pošta na odoslanie, až kým manuálne nespustíte operáciu odosielania a prijímania v programe Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
