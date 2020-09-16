---
title: 2491 upozorniť na e-mailové správy z Phish doručené z dôvodu politiky prepísania nájomníka alebo používateľa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728626"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorniť na e-mailové správy z Phish doručené z dôvodu politiky prepísania nájomníka alebo používateľa

Na nájomníkov s licenciami na Office 365 ATP P1 a P2 boli prevzaté predvolené politiky upozornení s názvom Phish doručené z dôvodu prepísania nájomníka alebo používateľa. Ak ste prijali toto upozornenie, tu sú uvedené kroky, ktoré je potrebné preskúmať:

1. V upozorňujúcej správe kliknite na položku **Zobraziť upozornenie** , čím prejdete na stránku **upozornenia** v centre zabezpečenia & dodržiavania súladu.

2. Vyberte upozornenie, aby sa zobrazila možnosť **Zobraziť zoznam správ** alebo **Zobraziť správy v Prieskumníkovi**. Obe tieto možnosti sa donesú do podrobností o správe, ktorá obsahuje identifikáciu správy. Všimnite si, že prepojenie na program Threat Explorer automaticky filtruje správy, ktoré zodpovedajú kritériám upozornenia. Možno bude potrebné nastaviť filter dátumu v programe Threat Explorer.

Správa neoprávneného získavania údajov bola doručená z dôvodu manuálne nakonfigurovaného prepísania:

- Povolený odosielateľ alebo doména, ktorú používateľ nastavil.

- Povoleného odosielateľa alebo domény nastavenej správcom v politike ochrany pred nevyžiadanou poštou.

- Povolená IP adresa v politike filtrovania pripojení.

- Pravidlo toku pošty (označuje sa aj ako pravidlo prenosu), ktoré je nakonfigurované na povolenie správ v programe.

Ak sa domnievate, že správa bola nesprávne označená ako Phish, na odoslanie vzoriek správ do spoločnosti Microsoft použite [doplnok správa zostavy](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programu Outlook.
