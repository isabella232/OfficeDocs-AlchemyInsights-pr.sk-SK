---
title: Synchronizácia hesla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960850"
---
# <a name="password-synchronization"></a>Synchronizácia hesla

**Synchronizácia hash hesiel vôbec nefunguje**

Niekoľko bežných problémov, s ktorými sa zákazníci stretávajú, keď synchronizácia hodnôt hash hesiel nefunguje, sú:

- Pre konto služby Active Directory používané službou Azure AD Pripojenie na  komunikáciu s lokálnou službou Active Directory nie je udelené povolenie replikovať zmeny adresárov a replikovať zmeny adresárov Všetky povolenia, ktoré sú potrebné na synchronizáciu hesiel – tento problém treba vyriešiť udelením týchto povolení pre konto služby Active Directory. 
- Synchronizácia hodnoty hash hesiel je vypnutá, keď  správca zmenil metódu používateľa Sign-In zo synchronizácie hesiel na inú možnosť, ako je napríklad federácia so službou **ADFS** v sprievodcovi Azure AD Pripojenie – tento problém môžete vyriešiť zapnutím funkcie synchronizácie hodnôt **hash** hesiel v sprievodcovi azure AD Pripojenie.
- Problém s pripojením s lokálnou službe Active Directory. Napríklad niektoré ovládače domén nie sú dostupné zo služby Azure [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) AD Pripojenie alebo sú nevyhnutné porty blokované bránou Firewall – tento problém treba vyriešiť tak, že zabezpečíte správne pripojenie medzi serverom služby Azure AD Pripojenie a lokálnou službou Active Directory.
- Server Azure AD Pripojenie je momentálne v režime opisu, čo bude mať za následok, že server nemôže získať hash hesiel. Pri riešení tohto problému postupujte podľa krokov popísaných v časti Riešenie problémov so synchronizáciou hesiel so službou Azure AD Pripojenie – nesynchronizujú sa žiadne [heslá.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Synchronizácia hash hesiel nefunguje pre niektorých používateľov**

1. Ak ste si všimli, že hodnota hash hesla  sa nesynchronizuje pre používateľa, pomocou úlohy riešenia problémov v nástroji Azure AD Pripojenie preskúmajte a vyriešte problém. Vykonajte tieto úlohy:

    a. [Spustenie úlohy na riešenie problémov v sprievodcovi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Problém so synchronizáciou hodnoty hash hesiel pre konkrétne použitie pomocou rutiny typu cmdlet na riešenie problémov](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Objekt lokálneho používateľa služby Active Directory je povolený pre **používateľa, musí zmeniť heslo pri najbližšom prihlásení.** Keď je táto možnosť povolená, používateľovi sa priradí dočasné heslo a pri ďalšom prihlásení sa zobrazí výzva na zmenu hesla. Azure AD Pripojenie nesynchronizuje dočasné heslá so službou Azure AD.

Problém môžete vyriešiť vykonaním jednej z nasledujúcich úloh:

- Požiadajte používateľa, aby sa prihlási do lokálnej aplikácie (napríklad Windows počítača) a zmenil heslo. Nové heslo sa zosynchronizuje so službou Azure AD.
- Umožniť správcovi aktualizovať heslo používateľa bez povolenia možnosti Používateľ musí pri najbližšom prihlásení zmeniť heslo a nové heslo zdieľať s používateľom.

3. Objekt lokálnej služby Active Directory User nie je **správne nakonfigurovaný na synchronizáciu** objektov alebo synchronizáciu hesla. Pri riešení tohto problému postupujte podľa krokov popísaných v časti Riešenie problémov so [synchronizáciou hodnoty hash hesiel so](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)službou Azure AD Pripojenie synchronizácie .







