---
title: Povoľte Trezor prílohy pre SharePoint Online, OneDrive a Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332394"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povoľte Trezor prílohy pre SharePoint Online, OneDrive a Microsoft Teams

1. Pomocou poverení globálneho správcu alebo správcu zabezpečenia otvorte portál Microsoft 365 Defender v systéme a potom prejdite na položku Politiky & pravidlá hrozieb <https://security.microsoft.com>  \>  \> **a Trezor Prílohy v** **časti** Politiky

   Ak chcete prejsť priamo na **Trezor prílohy,** použite <https://security.microsoft.com/safeattachmentv2> .

2. Na stránke **Trezor Prílohy** kliknite na položku **Globálne nastavenia**.
3. Na zobrazenom letáku vyberte položku Zapnúť Microsoft Defender pre Office 365 pre **SharePoint, OneDrive a Microsoft Teams** a potom vyberte položku **Uložiť**.

    **Tip:** Pomocou týchto krokov môžete vylepšiť ochranu osobných Trezor pre SharePoint, OneDrive a Microsoft Teams:
    - Ak chcete zabrániť používateľom v sťahovaní škodlivých súborov, použite hodnotu `$true` *parametra DisallowInfectedFileDownload* v rutine typu cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** v prostredí SharePoint Online PowerShell. Ďalšie informácie nájdete v téme [Použitie prostredia SharePoint Online PowerShell na zabránenie používateľom v sťahovaní škodlivých súborov.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Vytvorenie politiky upozornenia pre zistené súbory](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Ďalšie informácie nájdete v [téme Trezor prílohy pre Office 365 pre SharePoint, OneDrive a Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
