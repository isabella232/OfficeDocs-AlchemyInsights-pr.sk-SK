---
title: Premiestnenie e-mailových správ do archívnej poštovej schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522786"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premiestnenie e-mailu do archívnej poštovej schránky

Ak chcete, aby sme spúšťali automatizované kontroly nastavení uvedených nižšie, vyberte tlačidlo Späť < -- v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s presunom e-mailov do archívnej poštovej schránky.

1. Potvrďte, že **archívna poštová** schránka bola povolená. Ak nie, použite kroky v tomto [článku umožniť archívnej](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) poštovej schránky.

2. Ak chcete automaticky archivovať správy do archívnej poštovej schránky, značka uchovávania údajov s **akciou Premiestniť** do archívu musí byť nastavená **tak, aby sa automaticky použila na celú značku poštovej schránky (predvolenej)**. Ak chcete vytvoriť značku, použite kroky na vytvorenie [značky: Archivovať predvolenú značku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Potom pridajte značku **Archivovať** do politiky uchovávania údajov. V Centre spravovania pre Exchange vyberte **položku Politiky** uchovávania > **pridajte značku Presunúť** do archívu do politiky > **Uložiť**.

4. Teraz [priraďte politiku uchovávania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) údajov k poštovej schránke konkrétneho používateľa. Rovnaká politika sa použije na poštovú schránku **Primárne** aj **Archív.**

Môže byť potrebné vynútiť Asistenta pre spravované priečinky (MFA) spustiť a použiť nové nastavenia poštovej schránky používateľa. Spustite nasledujúci príkaz pri pripojení [k EXO PowerShell spustiť](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:
  
Štart-ManagedFolderAssistant -Identity<name of the mailbox>

Ďalšie informácie o nastavení politiky archivácie nájdete v téme [Nastavenie politiky archivácie a odstránenia poštových schránok](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  