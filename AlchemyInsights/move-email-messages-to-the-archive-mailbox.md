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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799795"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premiestnenie e-mailu do archívnej poštovej schránky

Ak chcete, aby sme spustili automatizované kontroly nižšie uvedených nastavení, vyberte tlačidlo späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s premiestnením e-mailov do svojej archívnej poštovej schránky.

1. Potvrďte, že je povolená **archívna poštová schránka** . Ak nie, použite postup v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) na povolenie archívnej poštovej schránky.

2. Ak chcete automaticky archivovať správy do archívnej poštovej schránky, značka uchovávania údajov s akciou **premiestniť do archívu** musí byť nastavená na možnosť **automaticky použiť na celú poštovú schránku (predvolená)**. Ak chcete vytvoriť značku, postupujte podľa týchto krokov: [Predvolená značka archivácie](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Potom pridajte značku **archivácie** do politiky uchovávania údajov. V centre spravovania pre Exchange vyberte položku **politiky uchovávania údajov** > pridať **značku premiestniť do archívu** do politiky > **Uložiť**.

4. Teraz [priraďte politiku uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) k poštovej schránke konkrétneho používateľa. Rovnaká politika sa použije na **primárnu** aj **archívnu** poštovú schránku.

Môže byť potrebné vynútiť Spustenie Asistenta pre spravované priečinky (MFA) a použiť nové nastavenia v poštovej schránke používateľa. Spustite nasledujúci príkaz pri [pripojení k EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) na spustenie Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:
  
Začiatok – ManagedFolderAssistant – identita <name of the mailbox>

Ďalšie informácie o nastavení politiky archivácie nájdete v téme [Nastavenie politiky archivácie a odstraňovania poštových schránok](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  