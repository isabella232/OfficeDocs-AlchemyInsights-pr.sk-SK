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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105773"
---
# <a name="troubleshoot-password-synchronization"></a>Riešenie problémov so synchronizáciou hesiel

Ak chcete riešiť problémy so synchronizáciou hesiel, začnite pomocou tejto úlohy služby AAD Pripojenie riešenie problémov s cieľom zistiť, prečo sa heslá nesynchronizujú. Ak chcete začať, prejdite na položku [Správa priamej synchronizácie](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorte novú reláciu Windows PowerShell na serveri Azure AD Pripojenie a vyberte **možnosť Spustiť ako** správca.

2. Spustite Set-ExecutionPolicy RemoteSigned alebo Set-ExecutionPolicy Unrestricted.

3. Spustite Sprievodcu Azure AD Pripojenie Ad.

4. Prejdite na stránku Ďalšie úlohy a vyberte > **Ďalej.**  >  

5. Výberom **položky Spustiť** otvorte ponuku na riešenie problémov v prostredí PowerShell.

6. Vyberte položku **Riešiť problémy so synchronizáciou hesiel**.

    Problém zvyčajne znamená, že heslo nie je synchronizované s konkrétnym používateľským kontom.

    **Poznámky** Ak posledná úspešná synchronizácia hesiel bola pred niekoľkými časmi, synchronizácia hesiel zlyhá.

Ďalšie informácie týkajúce sa riešenia problémov so synchronizáciou hesiel nájdete v téme Riešenie problémov so synchronizáciou hodnôt hash hesiel [so službou Azure AD Pripojenie synchronizácie](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).