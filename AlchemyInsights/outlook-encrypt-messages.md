---
title: S/MIME v Outlooku na webe
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772313"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifrovanie e-mailových správ v Outlooku

Šifrovanie správ v Microsoft 365 je postavené na lokalite Microsoft Azure Rights Management (Azure RMS), ktorá je súčasťou ochrany informácií Azure. Ak vaše predplatné zahŕňa Azure Rights Management alebo Azure Information Protection, **nemusíte vykonávať žiadne akcie na manuálne zapnutie alebo aktiváciu** služby správy prístupových práv.

Na základe pripomienok od zákazníkov už nebudeme povoľovať pravidlá toku pošty v Exchangei, aby sa predvolene automaticky zašifroval odchádzajúci e-mail obsahujúci určitý typ citlivých informácií v nájomníkovi. Namiesto toho poskytujeme podrobné pokyny o tom, ako môžete tak urobiť sami. Ďalšie podrobnosti o tom, ako vytvoriť pravidlo prenosu na šifrovanie citlivých informácií, nájdete v [tomto článku](https://aka.ms/OmeEtr).

- Ak používate Outlook na webe (predtým **OWA**): pri vytváraní e-mailovej správy jednoducho kliknite na položku **zabezpečiť** v aplikácii OWA. Použije sa povolenie na preposielanie ďalej. Kliknite na položku **zmeniť povolenie** a výberom položky **šifrovať** zašifrujete len správu.

- Ak používate **klienta Outlook**: Ak chcete odoslať šifrovanú správu z Outlooku 2013 alebo 2016 alebo Outlooku 2016 pre Mac **Options**, vyberte položku  >  **povolenia**pre možnosti a potom vyberte požadovanú možnosť ochrany.

- Ak chcete **automaticky šifrovať všetky e-maily** odoslané určitým príjemcom alebo externým partnerským organizáciám, musíte vytvoriť pravidlo prenosu toku pošty v centre spravovania pre Exchange. Podrobné pokyny sú uvedené v [tomto článku technickej podpory](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

