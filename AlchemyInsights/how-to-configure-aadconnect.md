---
title: 646 ako nakonfigurovať AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722578"
---
# <a name="configure-sync-features"></a>Konfigurácia funkcií synchronizácie

Azure AD Connect obsahuje niekoľko funkcií, ktoré sú predvolene povolené, alebo ktoré môžete povoliť neskôr. Niektoré funkcie vyžadujú dodatočnú konfiguráciu v konkrétnych prostrediach.

- [Filtrovanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obmedzuje objekty synchronizované Azure AD. Predvolene sa synchronizujú všetci používatelia, kontakty, skupiny a počítačové kontá systému Windows 10. Môžete zahrnúť alebo vylúčiť objekty na základe domén, OUs alebo iných atribútov.

- [Password hash synchronizácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hash hesla z lokálnej služby Active Directory Azure AD. To umožňuje správu hesiel na jednom mieste, ale použitie rovnakého hesla v lokálnom aj cloudovom prostredí. Keďže služba Active Directory je autoritatívnym zdrojom, môžete použiť vlastné heslo politiky.

- [Samoobslužné obnovenie hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje používateľom obnoviť svoje vlastné heslá v cloude, zatiaľ čo stále uplatňujú svoje lokálne heslo politiky.

- [Zariadenie writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje registrované zariadenia v Azure AD sa zapíše späť do lokálnej služby Active Directory tak môžu byť použité pre podmieneného prístupu.

- [Zabrániť náhodnému vymazaniu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je povolená v predvolenom nastavení zabrániť príliš veľa simultánne objekt odstránenia (viac ako 500 objektov na synchronizáciu). Toto nastavenie môžete zmeniť tak, aby spĺňate potreby vašej organizácie.

- [Automatická inovácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je predvolene povolená pre expresné inštalácie a pomáha zabezpečiť, aby vaša verzia Azure AD Connect bola vždy aktuálna.
