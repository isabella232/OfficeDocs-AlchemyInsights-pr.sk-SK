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
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511055"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premiestnenie e-mailu do archívnej poštovej schránky

1. Skontrolujte, či bola povolená **archívna poštová schránka.** Ak nie, použite kroky v [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) umožniť archívnej poštovej schránky.

2. Ak chcete automaticky archivovať správy do archívnej poštovej schránky, značka uchovávania údajov s akciou **Presunúť do archívu** musí byť nastavená tak, aby sa **automaticky použila na celú značku poštovej schránky (predvolenej).** Tu uvedené kroky vytvorte značku: [Predvolená značka archívu](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Potom pridajte značku **Archív** do politiky uchovávania údajov. V Centre spravovania pre Exchange vyberte položku **Politiky uchovávania údajov** > pridať **značku Presunúť do archívu** do politiky > **Uložiť**.

4. Teraz [priraďte politiku uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) k poštovej schránke konkrétneho používateľa. Rovnaká politika sa použije pre **poštovú** schránku Primárne aj **Archív.**

Môže byť potrebné vynútiť asistenta spravovaných priečinkov (MFA) spustiť a použiť nové nastavenia poštovej schránky používateľa. Spustite nasledujúci príkaz, keď [je pripojený k EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustiť Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:
  
Počiatočná Identifikácia programu ManagedFolderAssistant<name of the mailbox>

Ďalšie informácie o nastavení politiky archivácie sa nachádzajú v téme [Nastavenie politiky archivácie a odstránenia pre poštové schránky](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  