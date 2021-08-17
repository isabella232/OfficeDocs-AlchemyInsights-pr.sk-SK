---
title: 2491 Alert email messages from the 'Phish Delivered due to tenant or user override' policy
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
ms.openlocfilehash: 2e24f489292f38b5e9cacc8b9bfe5730ebfc71ce5e3004be479134ef6c791a12
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899347"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mailové správy s upozornením z politiky prepísania nájomníka alebo používateľa sa doručujú phish Delivered

Predvolená politika upozornenia s názvom **Phish Delivered z** dôvodu prepísania nájomníka alebo používateľa je k dispozícii v organizáciách s licenciami Microsoft Defender pre Office 365 P1 a P2. Ak ste dostali toto upozornenie, preskúmajte tieto kroky:

1. V upozornení kliknite na položku **Zobraziť upozornenie** a prejdite na **stránku** Upozornenia na portáli Microsoft 365 Defender upozornenia.

2. Ak chcete zobraziť možnosť Zobraziť zoznam správ alebo **Zobraziť správy v Prieskumníkovi,** **vyberte upozornenie.** Pomocou oboch týchto možností sa môžete o tejto správe postarať o podrobnosti, ktoré obsahujú identifikáciu správy. Všimnite si, že prepojenie Prieskumník hrozieb automaticky filtruje správy, ktoré spĺňajú kritériá upozornenia. Možno budete musieť upraviť filter dátumu v Prieskumníkovi hrozieb.

Správa s cieľom neoprávneného získavania údajov bola doručená z dôvodu manuálne nakonfigurovaného prepísania:

- Povolený odosielateľ alebo doména nastavená používateľom.
- Povolený odosielateľ alebo doména nastavená správcom v politike ochrany pred nevyžiadanou poštou.
- Povolená IP adresa v politike filtrovania pripojenia.
- Pravidlo toku pošty (známe aj ako pravidlo prenosu), ktoré je nakonfigurované na povolenie správ.

Ak si myslíte, že správa bola nesprávne označená ako neoprávnené získavanie údajov, na nahlásenie [správy](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) spoločnosti Microsoft použite odosielanie správcom.

Používatelia môžu na [odosielanie vzoriek](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) správ spoločnosti Microsoft použiť doplnok Nahlásiť správu alebo doplnok Nahlásiť neoprávnené získavanie údajov Outlook neoprávneného získavania údajov.
