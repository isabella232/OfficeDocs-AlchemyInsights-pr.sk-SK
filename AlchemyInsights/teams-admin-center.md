---
title: Centrum spravovania aplikácie Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354103"
---
# <a name="teams-admin-center"></a>Centrum spravovania aplikácie Teams

Získajte informácie o spravovaní aplikácie Teams s [Centrom spravovania aplikácie Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ak nemôžete získať prístup do Centra spravovania aplikácie Teams, skontrolujte tieto položky:

- Skontrolujte, či ste povolili zodpovedajúce [IP adresy balíka Office 365 a URL adresy](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v obvodových zariadeniach (firewall, atď.) alebo v pravidlách brány firewall vo vašom lokálnom počítači.
- Skontrolujte, či prihlasovacie meno, ktoré používate na prístup k portálu na správu tímov, zodpovedá vášmu používateľskému kontu uvedenému v [portáli pre správcov služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ak sa v Centre spravovania aplikácie Teams nezobrazujú používatelia, skontrolujte tieto položky:

- Vytvorili ste za posledných 24 hodín používateľov alebo priradili licencie? Uistite sa, že pred otvorením tiketu technickej podpory počkajte aspoň 24 hodín.
- Skontrolujte, či ste priradili zodpovedajúce licencie.
- Ak máte on-premise Active Directory, overiť, že [hodnota msRTCSIP-PrimaryUserAddress alebo adresu SIP v ProxyAddresses pole v lokálnej služby Active Directory je jedinečný a formát zodpovedá](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**používateľské meno** používateľa z [Microsoft 365 admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ak máte v úmysle udržať Skype Business Server nasadenie a používatelia homed lokálne a online: postupujte **"nastaviť hybridné tímy a Skype Business online"** Skype Business Server ovládací panel a presunúť používateľov online.
