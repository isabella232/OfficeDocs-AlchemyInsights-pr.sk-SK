---
title: Centrum spravovania aplikácie Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049359"
---
# <a name="teams-admin-center"></a>Centrum spravovania aplikácie Teams

Získajte informácie o spravovaní aplikácie Teams s [Centrom spravovania aplikácie Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ak nemôžete získať prístup do Centra spravovania aplikácie Teams, skontrolujte tieto položky:

- Skontrolujte, či ste povolili zodpovedajúce [IP adresy balíka Office 365 a URL adresy](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v obvodových zariadeniach (firewall, atď.) alebo v pravidlách brány firewall vo vašom lokálnom počítači.
- Skontrolujte, či prihlasovacie meno, ktoré používate na prístup k portálu na správu tímov, zodpovedá vášmu používateľskému kontu uvedenému v [portáli pre správcov služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ak sa v Centre spravovania aplikácie Teams nezobrazujú používatelia, skontrolujte tieto položky:

- Vytvorili ste za posledných 24 hodín používateľov alebo priradili licencie? Uistite sa, že pred otvorením tiketu technickej podpory počkajte aspoň 24 hodín.
- Skontrolujte, či ste priradili zodpovedajúce licencie.
- Ak máte lokálnu active directory, overte, či je hodnota [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) alebo adresa SIP v poli ProxyAddresses v lokálnej službe Active Directory jedinečná a formát zodpovedá sip: Meno používateľa z [konta Centrum spravovania služby Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Ak plánujete nasadenie služby Skype for Business Server a máte používateľov lokálne a online: postupujte podľa krokov v časti **Nastavenie hybridného** nasadenia so systémom Teams a Skype for Business Online na ovládacom paneli služby Skype for Business Server a presuňte používateľov online.
