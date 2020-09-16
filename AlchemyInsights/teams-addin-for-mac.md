---
title: Doplnok teams pre Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670343"
---
# <a name="teams-add-in-for-mac"></a>Doplnok teams pre Mac

Ak chcete vyriešiť problém s chýbajúcimi tímami pre používateľov operačných systémov pre Mac, postupujte takto:

**Krok 1:** Ak máte lokálne hybridné Exchange (2016 CU3 alebo novšiu verziu), pomocou nástroja Test-HMA.ps1 potvrďte, že hybridné moderné overovanie je správne nakonfigurované. Ďalšie informácie nájdete v téme [overovanie hybridného moderného nastavenia overovania pre Outlook pre iOS a Android](https://aka.ms/AA980zq).  

**Poznámka:** Použite formát adresy UPN (napríklad [username@contoso.com](mailto:username@contoso.com)), nie Domain\Username. Urobte to aj pre používateľov s poštovými schránkami v službe Exchange Online.

**Krok 2:** Používateľ musí prejsť na kontá **nástrojov**  >  **Accounts**... v Outlooku pre Mac a vyhľadajte a vyberte konto. Potvrďte, že je uvedené meno používateľa vo formáte UPN (napríklad [username@contoso.com](mailto:username@contoso.com)).

**Krok 3:** Potvrďte, že používateľ je licencovaným používateľom aplikácie Microsoft teams. Používateľ musí používať predplatné na Office 365 pre Mac, verziu produktu 16,24 alebo novšiu verziu.