---
title: Centrum spravovania aplikácie Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670379"
---
# <a name="teams-admin-center"></a>Centrum spravovania aplikácie Teams

Získajte informácie o spravovaní aplikácie Teams s [Centrom spravovania aplikácie Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ak nemôžete získať prístup do Centra spravovania aplikácie Teams, skontrolujte tieto položky:

- Skontrolujte, či ste povolili zodpovedajúce [IP adresy balíka Office 365 a URL adresy](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v obvodových zariadeniach (firewall, atď.) alebo v pravidlách brány firewall vo vašom lokálnom počítači.
- Skontrolujte, či prihlasovacie meno, ktoré používate na prístup k portálu na správu tímov, zodpovedá vášmu používateľskému kontu uvedenému v [portáli pre správcov služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ak sa v Centre spravovania aplikácie Teams nezobrazujú používatelia, skontrolujte tieto položky:

- Vytvorili ste za posledných 24 hodín používateľov alebo priradili licencie? Uistite sa, že pred otvorením tiketu technickej podpory počkajte aspoň 24 hodín.
- Skontrolujte, či ste priradili zodpovedajúce licencie.
- Ak máte lokálnu službu Active Directory, overte, či [je v poli proxyAddresses v lokálnej službe Active Directory hodnota msRTCSIP-PrimaryUserAddress alebo adresa SIP, ktorá sa zhoduje s formátom](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**meno** používateľa používateľa z [centra spravovania služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ak máte v úmysle uchovať nasadenie Skypu for Business Server a mať používateľov doma lokálne a online: postupujte podľa pokynov v časti **Nastavenie hybridného nasadenia v aplikácii teams a Skype for Business online** v ovládacom paneli Skypu for Business Server a premiestnite používateľov online.
