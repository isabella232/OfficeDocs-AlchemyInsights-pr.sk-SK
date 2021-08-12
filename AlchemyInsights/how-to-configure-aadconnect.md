---
title: 646 Konfigurácia služby AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963658"
---
# <a name="configure-sync-features"></a>Konfigurácia funkcií synchronizácie

Azure AD Pripojenie obsahuje niekoľko predvolene povolených funkcií alebo ktoré môžete zapnúť neskôr. Niektoré funkcie vyžadujú dodatočnú konfiguráciu v konkrétnych prostrediach.

- [Obmedzenia filtrovania](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objektov sa synchronizujú so službou Azure AD. Predvolene sa synchronizujú všetci používatelia, kontakty, Windows 10 a kontá počítačov. Objekty založené na doménach, OU alebo iných atribútoch môžete zahrnúť alebo vylúčiť.

- [Synchronizácia hodnoty hash hesla](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hodnotu hash hesla z lokálnej služby Active Directory so službou Azure AD. Toto umožňuje správu hesiel na jednom mieste, ale používanie rovnakého hesla v lokálnych aj cloudových prostrediach. Keďže Active Directory je autoritatívnym zdrojom, môžete použiť vlastné politiky hesiel.

- [Samoobslužné vytvorenie nového hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje používateľom vytvárať si nové heslá v cloude a zároveň uplatňovať lokálnu politiku hesiel.

- [Funkcia Writeback zariadenia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje zapisovanie zaregistrovaných zariadení v službe Azure AD späť do lokálnej služby Active Directory, aby ich bolo možné použiť na podmienený prístup.

- [Zabránenie neúmyselným odstráneniám je](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) predvolene povolené, aby sa zabránilo príliš veľkému súčasnému odstraňovaniu objektov (viac než 500 objektov na synchronizáciu). Toto nastavenie môžete zmeniť tak, aby vyhovovalo potrebám vašej organizácie.

- [Automatická](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) inovácia je predvolene povolená pre expresné inštalácie a pomáha zabezpečiť, aby vaša verzia služby Azure AD Pripojenie bola vždy aktuálna.
