---
title: S/MIME v programe Outlook na webe
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752875"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifrovať e-mailové správy v programe Outlook

Office 365 šifrovanie správ je postavená na Microsoft Azure Rights Management (Azure RMS), ktorý je súčasťou Azure Information Protection. Ak vaše predplatné zahŕňa Azure Rights Management alebo Azure ochranu informácií, nemusíte **podniknúť žiadne kroky na manuálne povolenie alebo aktiváciu** služby správy prístupových práv.

Na základe spätnej väzby od zákazníkov už nebudeme umožňovať pravidlá toku poštových služieb Exchange, aby sa automaticky zašifrovali odchádzajúce e-maily obsahujúce určitý typ citlivých informácií v nájomníkovi predvolene. Namiesto toho poskytujeme podrobné pokyny, ako to môžete urobiť sami. Ďalšie informácie o tom, ako vytvoriť pravidlo prenosu na zašifrovanie citlivých informácií, nájdete [v tomto článku](https://aka.ms/OmeEtr).

- Ak používate program Outlook na webe (predtým **OWA**): pri vytváraní e-mailovej správy, jednoducho kliknite na tlačidlo **chrániť** v aplikácii OWA. Toto bude platiť povolenie "Neposielať ďalej". Kliknite na tlačidlo **zmeniť povolenie** a vyberte **Zašifrovať** len zašifrovať správy.

- Ak používate **klienta Outlook**: Ak chcete odoslať zašifrovanú správu z programu Outlook 2013 alebo 2016, alebo Outlook 2016 pre Mac, vyberte **Možnosti** > **povolenia**, potom vyberte možnosť ochrany, ktorú potrebujete.

- Ak chcete **automaticky zašifrovať všetky e-maily** odoslané určitým príjemcom alebo externým partnerským organizáciám, musíte v stredisku Exchange Admin Center vytvoriť pravidlo prenosu pošty. Podrobné inštrukcie sú uvedené v [tomto článku podpory](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

