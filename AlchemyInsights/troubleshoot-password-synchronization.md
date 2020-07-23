---
title: Riešenie problémov so synchronizáciou hesiel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387892"
---
# <a name="troubleshoot-password-synchronization"></a>Riešenie problémov so synchronizáciou hesiel

Ak chcete riešiť problémy so synchronizáciou hesiel, začnite pomocou tejto úlohy riešenia problémov AAD Connect a zistite, prečo sa heslá nesynchronizujú. Ak chcete začať, prejdite na [Spravovať priamu synchronizáciu](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorte novú reláciu prostredia Windows PowerShell na serveri Azure AD pripojiť a vyberte **možnosť Spustiť ako** správca .

2. Spustiť Set-ExecutionPolicy RemoteSigned alebo Set-ExecutionPolicy Neobmedzený.

3. Spustite Sprievodcu pripojením Azure AD.

4. Prejdite na stránku Ďalšie úlohy a > riešenie **problémov s ďalším**  >  **Next**.

5. Výberom položky **Launch** (Spustiť) otvorte ponuku na riešenie problémov v prostredí PowerShell.

6. Vyberte **položku Riešenie problémov so synchronizáciou hesiel**.

    Problém je zvyčajne, že heslo nie je synchronizovaný pre konkrétne používateľské konto.

    **Poznámky k používaniu** Synchronizácia hesiel zlyhá, ak bola posledná úspešná synchronizácia hesla pred nejakým časom.

Ďalšie informácie o riešení problémov so synchronizáciou hesiel nájdete v [téme Riešenie problémov so synchronizáciou hash hesla pomocou synchronizácie služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).