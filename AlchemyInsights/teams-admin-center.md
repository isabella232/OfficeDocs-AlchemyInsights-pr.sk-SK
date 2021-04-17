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
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826394"
---
# <a name="teams-admin-center"></a>Centrum spravovania aplikácie Teams

Získajte informácie o spravovaní aplikácie Teams s [Centrom spravovania aplikácie Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ak nemôžete získať prístup do Centra spravovania aplikácie Teams, skontrolujte tieto položky:

- Skontrolujte, či ste povolili zodpovedajúce [IP adresy balíka Office 365 a URL adresy](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v obvodových zariadeniach (firewall, atď.) alebo v pravidlách brány firewall vo vašom lokálnom počítači.
- Skontrolujte, či prihlasovacie meno, ktoré používate na prístup k portálu na správu tímov, zodpovedá vášmu používateľskému kontu uvedenému v [portáli pre správcov služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ak sa v Centre spravovania aplikácie Teams nezobrazujú používatelia, skontrolujte tieto položky:

- Vytvorili ste za posledných 24 hodín používateľov alebo priradili licencie? Uistite sa, že pred otvorením tiketu technickej podpory počkajte aspoň 24 hodín.
- Skontrolujte, či ste priradili zodpovedajúce licencie.
- Ak máte lokálnu službu Active Directory, overte, či je hodnota [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) alebo adresa SIP v poli ProxyAddresses v lokálnej službe Active Directory jedinečná a formát zodpovedá sip: Meno používateľa z Centra spravovania služby [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Ak plánujete nasadenie Skype for Business Servera a máte používateľov lokálne a online, postupujte podľa krokov v časti **Nastavenie hybridného** nasadenia s aplikáciami Teams a Skype for Business Online na ovládacom paneli Skype for Business Servera a presuňte používateľov online.
