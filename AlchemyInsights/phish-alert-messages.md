---
title: 2491 upozorňujúce e-mailové správy z "Phish dodané z dôvodu nájomcu alebo používateľ prepísať" politiky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758948"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorňujúce e-mailové správy z ' Phish dodané z dôvodu nájomcu alebo používateľ prepísať ' politika

Predvolená politika upozornenia s názvom "Phish dodané z dôvodu nájomcu alebo prepísať používateľa" bola vrátená nájomníkmi s Office 365 ATP P1 a P2 licencie. Ak ste dostali Toto upozornenie, tu sú kroky na vyšetrenie:

1. Z upozorňujúce hlásenie, kliknite na tlačidlo **Zobraziť upozornenie** prejdite na stránku **upozornenia** v zabezpečenie & Compliance Center.

2. Vyberte upozornenie, ak chcete zobraziť možnosť **zobrazenia zoznamu správ** alebo **Zobraziť správy v Prieskumníkovi**. Obe tieto možnosti sa dostanete na Podrobnosti správy, ktorá obsahuje ID správy. Všimnite si, že hrozba Explorer odkaz bude automaticky filtrovať správy, ktoré zodpovedajú výstražné kritériá. Možno bude potrebné upraviť filter dátumu v programe Threat Explorer.

Hlásenie neoprávneného získavania údajov bolo dodané z dôvodu manuálne nakonfigurovaného prepísania:

- Povolený odosielateľ alebo doména nastavená používateľom.

- Povolený odosielateľ alebo doména nastavená správcom v politike anti-spam.

- Povolená adresa IP v politike filtra pripojenia.

- Pravidlo toku pošty (známe aj ako pravidlo prenosu), ktoré je nakonfigurované na povolenie správ.

Ak sa domnievate, že správa bola nesprávne označená ako Phish, použite [doplnok](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) správy programu Outlook na odoslanie vzoriek správ spoločnosti Microsoft.
