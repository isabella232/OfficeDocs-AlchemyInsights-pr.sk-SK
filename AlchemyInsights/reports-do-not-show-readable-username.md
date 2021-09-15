---
title: V zostavách v Centre spravovania služby Microsoft 365 sa nezobrazuje čitateľné meno používateľa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327829"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>V zostavách v Centre spravovania služby Microsoft 365 sa nezobrazuje čitateľné meno používateľa

V zostavách v Centre spravovania služby Microsoft 365 sa nezobrazujú mená používateľov, ale zobrazujú sa namiesto nich alfanumerické hodnoty, napríklad B2BC6C15BB9FCDEA71E5CD302D228CC8.

Ide o očakávané správanie, ktoré bolo oznámené v centre správ (MC275344, publikované 3. augusta 2021). 

Globálni správcovia môžu túto zmenu pre svojho nájomníka vrátiť a zobraziť identifikovateľné informácie o používateľoch, ak to umožňujú zásady ochrany osobných údajov ich organizácie. Ak chcete pre nájomníka vrátiť zmenu:

1. V centre spravovania prejdite do časti **Nastavenia** > **Nastavenia organizácie** > [**Služby**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) a vyberte položku **Zostavy**. 
1. V časti **Vyberte spôsob zobrazenia informácií o používateľoch** vyberte položku **Zobraziť identifikovateľné informácie o používateľoch v zostavách** a potom zostavu znova spustite.