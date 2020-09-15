---
title: 646 ako nakonfigurovať AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704504"
---
# <a name="configure-sync-features"></a>Konfigurácia funkcií synchronizácie

Azure AD Connect obsahuje niekoľko funkcií, ktoré sú predvolene zapnuté, alebo ktoré môžete neskôr povoliť. Niektoré funkcie vyžadujú ďalšiu konfiguráciu v konkrétnych prostrediach.

- [Filtrovanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obmedzení objekty sa synchronizujú so službou Azure AD. Predvolene sa synchronizujú všetci používatelia, kontakty, skupiny a kontá počítačov s Windowsom 10. Môžete zahrnúť alebo vylúčiť objekty na základe domén, organizačných jednotkí alebo iných atribútov.

- [Synchronizácia hash hesla](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hash hesla z lokálnej služby Active Directory do služby Azure AD. To umožňuje správu hesiel na jednom mieste, ale použitie rovnakého hesla v lokálnom aj cloudovom prostredí. Keďže Active Directory je autoritatívnym zdrojom, môžete použiť vlastné politiky hesiel.

- [Samoobslužné vytvorenie nového hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje používateľom vytvoriť si nové heslá v cloude a zároveň použiť politiku lokálneho hesla.

- [Zariadenie zápisom](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje zapísať do lokálnej služby Active Directory registrované zariadenia v službe Azure AD, aby sa mohli použiť na podmienený prístup.

- [Predchádzanie náhodným](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) odstránením je predvolene zapnuté, aby sa predišlo príliš mnohým súčasným odstránením objektov (viac než 500 objektov na synchronizáciu). Toto nastavenie môžete zmeniť tak, aby vyhovovalo potrebám vašej organizácie.

- [Automatická inovácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je predvolene zapnutá pri expresných inštaláciách a pomáha zabezpečiť, že vaša verzia služby Azure AD Connect je vždy aktuálna.
