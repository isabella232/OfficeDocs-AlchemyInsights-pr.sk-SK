---
title: Presunúť e-mailových správ do archívnej poštovej schránky
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
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36549019"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premiestniť e-mail do archívnej poštovej schránky

1. Potvrdiť, že bola povolená **archivácia poštovej schránky** . Ak nie, použite kroky v [tomto článku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) na zapnutie archívnej poštovej schránky.

2. Archív správ automaticky do archívnej poštovej schránky, značku uchovávania údajov s akciou **, premiestniť do archívu** musí stanoviť uplatňovať **automaticky tag celý schránky (predvolené)**. Použite kroky tu vytvoriť značku: [Archív predvolené tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Ďalej pridať **Archív** značku k politike uchovávania údajov. Admin Center Exchange, vybrať **Uchovávanie podmienky** > pridať, **premiestniť do archívu značky** politiky > **Uložiť**.

4. Teraz [priraďte politiku uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštovej schránky špecifické používateľa. **Primárnej** a **archívnej** poštovej schránky sa použije rovnakú politiku.

Môže byť potrebné prinútiť podarilo priečinka asistent (MFA) spustiť a použiť nové nastavenia do poštovej schránky používateľa. Spustite nasledujúci príkaz zároveň [pripojený k EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustiť Asistenta pre spravované priečinky v konkrétnej poštovej schránke:
  
Štart-ManagedFolderAssistant-Identity<name of the mailbox>

Ďalšie informácie o nastavení politiku archivácie, v téme [Set up Archív a odstránenie politiky poštových schránok](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  