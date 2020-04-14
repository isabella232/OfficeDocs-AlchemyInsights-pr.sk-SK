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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241267"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Oprava správ, ktoré sú prilepené v priečinku Pošta na odoslanie

Odporúčame vám začať spustením scenára ["Mám problémy s odosielaním, prijímaním alebo vyhľadávaním e-mailových správ"](https://aka.ms/SaRA-OutlookSendReceive) z nástroja [technickej podpory a obnovenia programu Microsoft](https://diagnostics.office.com/#/) .

Keď správa uviazne v priečinku Pošta na odoslanie, najpravdepodobnejšou príčinou je veľká príloha alebo možnosť "Odoslať ihneď po pripojení" nie je povolená.

**Odstráňte veľkú prílohu**

1. V programe Outlook vyberte položku **Odoslať a prijať** > **prácu v režime offline**. 
2. Na navigačnej table vyberte položku **Pošta na odoslanie**. Odtiaľ môžete: 
    - Odstráňte správu (vyberte ju a potom vyberte položku **Delete**).
    - Presuňte správu do priečinka Koncepty, dvojitým kliknutím ho otvorte a odstráňte ju vyberte a potom vyberte položku **Delete (odstrániť**).
3. Ak sa zobrazí chyba, ktorá hovorí, že program Outlook sa pokúša odovzdať správu, zavrite program Outlook. Ukončenie môže trvať niekoľko okamihov. Ak sa program Outlook nezavrie, stlačte kombináciu klávesov CTRL + ALT + DELETE a vyberte položku **Spustiť správcu úloh**. V Správcovi úloh vyberte kartu **procesy** , posuňte sa nadol do programu Outlook. exe a vyberte položku **ukončiť proces**.
4. Po zatvorení programu Outlook, reštartujte ho a zopakujte kroky 2 a 3. 
5. Po odstránení prílohy kliknite na položku **Odoslať a prijať** > **prácu v režime offline** a pokračujte v práci online. 

Správy tiež uviaznu v priečinku Pošta na odoslanie po kliknutí na tlačidlo **Odoslať**, ale nie ste pripojení. Kliknite na tlačidlo **Odoslať a prijať** a pozrite sa na tlačidlo **pracovať v režime offline** . Ak je modrá, ste odpojený. Kliknutím naň sa pripojíte (tlačidlo sa zmení na bielu) a kliknite na tlačidlo **Odoslať všetko**.
 
**Povoliť odosielanie ihneď po pripojení**
 
1. Na súbor karte, kliknite na tlačidlo **Možnosti**.

2. V dialógovom okne Možnosti programu Outlook kliknite na tlačidlo **Spresniť**.

3. V časti Odoslať a prijať kliknutím povoľte **Odoslať ihneď po pripojení**. Kliknite na tlačidlo **OK**.
 
Podrobné informácie nájdete na:
- [Video: odoslanie alebo odstránenie uviaznutia e-mailu](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-mail zostane v priečinku Pošta na odoslanie, až kým manuálne nespustíte operáciu odosielania a prijímania v programe Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
