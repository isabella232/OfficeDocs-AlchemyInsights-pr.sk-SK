---
title: Riešenie problémov so synchronizáciou hesiel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664941"
---
# <a name="troubleshoot-password-synchronization"></a>Riešenie problémov so synchronizáciou hesiel

Ak chcete riešiť problémy so synchronizáciou hesiel, začnite pomocou tohto nástroja AAD pripojiť riešenie problémov a zistite, prečo sa heslá nesynchronizujú. Ak chcete začať, prejdite na položku [Správa priamej synchronizácie](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorte novú reláciu prostredia Windows PowerShell na serveri Azure AD Connect a vyberte možnosť **Spustiť ako správca** .

2. Spustite set-ExecutionPolicy RemoteSigned alebo set-ExecutionPolicy neobmedzený.

3. Spustite Sprievodcu Azure AD Connect.

4. Prejdite na stránku ďalšie úlohy > **Riešenie problémov s**  >  **ďalšou**.

5. Ak chcete otvoriť ponuku riešenie problémov v prostredí PowerShell, vyberte položku **Spustiť** .

6. Vyberte položku **Riešenie problémov so synchronizáciou hesiel**.

    Problém je zvyčajne to, že heslo nie je synchronizované pre konkrétne používateľské konto.

    **Poznámky** Synchronizácia hesiel zlyhá, ak bola Posledná úspešná synchronizácia hesiel pred nejakým časom.

Ďalšie informácie o riešení problémov so synchronizáciou hesiel nájdete v téme [Riešenie problémov so synchronizáciou hash hesla pomocou synchronizácie služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).