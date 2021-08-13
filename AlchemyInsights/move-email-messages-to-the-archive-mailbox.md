---
title: Premiestnenie e-mailových správ do archívnej poštovej schránky
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974972"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premiestnenie e-mailu do archívnej poštovej schránky

Ak chcete, aby sme spúšťali automatické kontroly nižšie uvedených nastavení, vyberte tlačidlo Späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s premiestnením e-mailov do archívnej poštovej schránky.

1. Skontrolujte, či je **archívna poštová** schránka povolená. Ak nie, podľa krokov v tomto [článku povoľte](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) archívne poštové schránky.

2. Ak chcete automaticky archivovať správy do archívnej poštovej schránky, je nutné nastaviť značku uchovávania údajov s ak chcete, aby sa správy automaticky použili na celú  **(predvolenú) značku uchovávania údajov.** Ak chcete vytvoriť značku, postupujte takto: [Predvolená značka archivácie](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Potom k politike **uchovávania** údajov pridajte značku Archív. V Centre Exchange vyberte položku Politiky uchovávania **údajov** a  > k politike pridajte značku Premiestniť do archívu > **Uložiť**.

4. Teraz [priraďte politiku uchovávania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) údajov k poštovej schránke konkrétneho používateľa. Rovnaká politika sa použije na primárnu aj **archívne** **poštovú schránku.**

Môže byť potrebné vynútiť spustenie a použitie nových nastavení asistenta spravovaných priečinkov v poštovej schránke používateľa. Po pripojení k [EXO PowerShell spustite](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) tohto príkazu a spustite asistenta spravovaných priečinkov pre konkrétnu poštovú schránku:
  
Start-ManagedFolderAssistant – identita <name of the mailbox>

Ďalšie informácie o nastavení politiky archivácie nájdete v téme [Nastavenie politiky archivácie a odstraňovania pre poštové schránky.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  