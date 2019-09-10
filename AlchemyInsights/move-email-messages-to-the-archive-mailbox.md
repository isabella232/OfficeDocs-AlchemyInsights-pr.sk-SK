---
title: Presun e-mailových správ do archívnej poštovej schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822177"
---
# <a name="move-email-to-the-archive-mailbox"></a>Presunutie e-mailu do archívnej poštovej schránky

1. Skontrolujte, či bola povolená **archívna poštová schránka** . Ak nie, použite kroky v [tomto článku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) na povolenie archívnej poštovej schránky.

2. Ak chcete archivovať správy automaticky do archívnej poštovej schránky, značka uchovávania údajov s akciou **premiestniť do archívu** musí byť nastavená tak, aby sa **automaticky uplatňovala na celú poštovú schránku (predvolenú) značku**. Pomocou krokov tu vytvorte Tag: [Archivovať predvolenú značku](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Potom pridajte **archívnu** značku do politiky uchovávania údajov. Exchange Admin Center, vyberte **politiky uchovávania údajov** > pridať **presunúť do archívu Tag** politiky > **Uložiť**.

4. Teraz [priraďte politiku uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkrétnej poštovej schránke používateľa. Rovnaká politika sa použije ako **primárna** aj **archívna** poštová schránka.

Môže byť potrebné vynútiť Asistenta spravovaných priečinkov (MFA) spustiť a použiť nové nastavenia poštovej schránky používateľa. Spustite nasledujúci príkaz pri [pripojení k EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustiť Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:
  
Štart-ManagedFolderAssistant-identity<name of the mailbox>

Ďalšie informácie o nastavení politiky archivácie nájdete [v téme Nastavenie politiky archivácie a odstránenia poštových schránok](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  