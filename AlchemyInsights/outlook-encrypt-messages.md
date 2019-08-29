---
title: S/MIME v programe Outlook na webe
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666855"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifrovanie e-mailových správ v programe Outlook

Šifrovanie správ v Office 365 je postavený na Microsoft Azure Rights Management (Azure RMS), ktorá je súčasťou Azure ochranu informácií. Ak vaše predplatné obsahuje Azure Rights Management alebo Azure ochrana informácií, **nie je potrebné podniknúť akékoľvek opatrenia manuálne povoliť alebo aktivovať** správy prístupových práv.

Na základe spätnej väzby od zákazníkov, sme sa už umožňujúce Exchange mail tok pravidiel na automatické šifrovanie odchádzajúce e-mail obsahujúci určitý druh citlivé informácie v nájomcu v predvolenom nastavení. Namiesto toho poskytujeme podrobné pokyny o ako môžete tak urobiť sami. Ďalšie podrobnosti o tom, ako vytvoriť pravidlo dopravy šifrovať citlivé údaje, nájdete v [tomto článku](https://aka.ms/OmeEtr).

- Ak používate program Outlook na webe (predtým **OWA**): pri písaní e-mailovej správy, stačí kliknúť **Ochrana** v OWA. To sa vzťahuje povolenie "Do not forward". Kliknite na položku **zmeniť povolenie** a vyberte voľbu **Zašifrovať** iba šifrovanie správy.

- Ak používate **klienta Outlook**: odoslať šifrovanú správu z programu Outlook 2013 alebo 2016 alebo Outlook 2016 for Mac, vyberte polo¾ku **Voåby** > **povolenia**a potom vyberte možnosť ochrany, ktoré potrebujete.

- Na **automatické šifrovanie všetkých e-mailov** odoslané do určitých príjemcov alebo externej partnerskej organizácie, musíte vytvoriť pravidlo prenosu pošty toku v Exchange Admin Center. Podrobné pokyny sú uvedené v [tomto článku technickej podpory](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

