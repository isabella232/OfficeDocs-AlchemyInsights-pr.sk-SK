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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483083"
---
# <a name="password-synchronization"></a>Synchronizácia hesla

**Synchronizácia hash hesla nefunguje vôbec**

Niektoré bežné problémy, s ktorými sa zákazníci stretávajú, keď Synchronizácia hash hesla nefunguje:

- Konto služby Active Directory používané službou Azure AD Connect na komunikáciu s lokálnou službou Active Directory neposkytuje **replikovať zmeny adresárov** a **replikovať zmeny v adresári všetky** povolenia, ktoré sú potrebné na synchronizáciu hesla – musíte tento problém vyriešiť tak, že udelíte tieto povolenia do konta služby Active Directory.
- Synchronizácia hash hesla je vypnutá, keď správca zmenil používateľa Sign-In metódu z **synchronizácie hesiel** na inú možnosť, ako napríklad **federácia s AD FS** v sprievodcovi Azure AD Connect – tento problém môžete opraviť opätovným zapnutím funkcie **synchronizácie hash hesla** v sprievodcovi Azure AD Connect.
- Problém s pripojením s lokálnou službou Active Directory. Niektoré radiče domén napríklad nie sú prístupné prostredníctvom služby Azure AD Connect, prípadne porty, ktoré [vyžaduje](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) brána firewall, je potrebné vyriešiť tak, že zabezpečíte, že pripojenie medzi SERVEROM Azure AD Connect a lokálnou službou Active Directory funguje správne.
- Azure AD Connect server sa momentálne nachádza v režime staging, čo bude mať za následok, že server neumožňuje hash hesla – na vyriešenie problému postupujte podľa krokov uvedených v časti [Riešenie problémov so synchronizáciou hesiel pomocou služby Azure AD Connect Sync – žiadne heslá sa nesynchronizujú](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Synchronizácia hash hesla nefunguje pre niektorých používateľov**

1. Ak ste si všimli, že hash hesla sa pre používateľa nesynchronizuje, použite **Riešenie problémov** s úlohou v službe Azure AD Connect, aby sa problém vyriešil. Vykonajte tieto úlohy:

    a. [Spustenie úlohy riešenia problémov v sprievodcovi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Použite rutinu typu cmdlet na riešenie problémov a Preskúmajte problém s synchronizáciou hash hesla pre konkrétne použitie.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Lokálny objekt používateľa služby Active Directory je zapnutý, aby **používateľ musel zmeniť heslo pri ďalšom prihlásení** . Keď je táto možnosť povolená, používateľovi sa priradí dočasné heslo a pri ďalšom prihlásení sa zobrazí výzva na zmenu hesla. Azure AD Connect nesynchronizuje dočasné heslá na Azure AD.

Ak chcete vyriešiť tento problém, vykonajte jednu z nasledujúcich úloh:

- Požiadajte používateľa, aby sa prihlásil do lokálnej aplikácie (napríklad na pracovnej ploche Windowsu), a zmeňte heslo. Nové heslo sa synchronizuje so službou Azure AD.
- Požiadajte správcu o aktualizáciu hesla používateľa bez toho, aby ste museli povoliť používateľovi možnosť pri **ďalšom prihlásení zmeniť heslo** a nové heslo zdieľať s používateľom.

3. Objekt používateľa lokálnej služby Active Directory **nie je správne nakonfigurovaný** na synchronizáciu objektov alebo synchronizáciu hesla. Ak chcete vyriešiť tento problém, postupujte podľa krokov uvedených v [téme Riešenie problémov so synchronizáciou hash hesla pomocou služby Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







