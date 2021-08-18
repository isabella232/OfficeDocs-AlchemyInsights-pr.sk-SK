---
title: OneDrive prihlásenia AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112927"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive prihlásenia AADSTS50011

Ak sa pri prihlasovaní do aplikácie OneDrive zobrazí chyba "AADSTS50011: URL adresa odpovede zadaná v žiadosti nezodpovedá odpovedi", skontrolujte, či:

Vaša OneDrive musí byť rovnaká alebo novšia ako verzia 20.052.XXXX.XXXX. Ak chcete skontrolovať svoju verziu, kliknite na OneDrive ikonu oznámení v oblasti oznámení, vyberte položku **Pomocník a & Nastavenia > Nastavenia > Informácie.**

Sieť môže blokovať prenos údajov **do služieb g.live.com** a **oneclient.sfx.ms**. Ak je prenos zablokovaný, OneDrive nemôže aktualizovať. Ak chcete zabezpečiť prístup k týmto URL adresách, pracujte so správcom siete. [Tieto koncové body](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) by mali byť dostupné pre zákazníkov, ktorí používajú Microsoft 365 plány.

Ak potrebujete získať aktuálnu verziu Balíka Office OneDrive, navštívte lokalitu [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
