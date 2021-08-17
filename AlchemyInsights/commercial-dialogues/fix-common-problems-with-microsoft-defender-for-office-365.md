---
title: Riešenie bežných problémov s programom Microsoft Defender pre Office 365
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
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898259"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Riešenie bežných problémov s programom Microsoft Defender pre Office 365

Tu je niekoľko riešení bežných problémov s programom Microsoft Defender pre Office 365:

- **Oneskorenie správy:**

  Oneskorenia v doručovaní e-mailov môžu spôsobovať Trezor Kontrola príloh správ. Ďalšie informácie nájdete v téme [Trezor nastavenia politiky prílohy.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Hlásenie nesprávne pozitívnych alebo záporných výsledkov:**

  Ďalšie informácie nájdete v téme [Nahlásenie správ a súborov spoločnosti Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Zapnúť Trezor prepojenie:**

  1. Na portáli Microsoft 365 Defender prejdite na položku E-mailové politiky spolupráce pre & e-mailom & Pravidlá pravidiel <https://security.microsoft.com/>  \>  \>  \> **hrozieb Trezor Prepojenia** v **časti** Politiky.

     Ak chcete prejsť priamo na **Trezor prepojenia,** <https://security.microsoft.com/safelinksv2> použite .

  2. Na **Trezor** Prepojenia vyberte politiku kliknutím na názov politiky.
  3. V zobrazenej bubline podrobností vykonajte niektorý z týchto krokov:
     - Ak chcete pridať novú politiku, vyberte položku **+ Vytvoriť**. Spustí sa sprievodca, ktorý vám pomôže definovať nastavenia politiky.
     - Ak chcete upraviť existujúcu politiku, vyberte politiku kliknutím na jej názov. V zobrazenej bubline s podrobnosťami vyberte položku **Upraviť v** **časti Nastavenia** ochrany.
  4. Na stránke **Nastavenia ochrany** nakonfigurujte tieto nastavenia:
     - Zapnite **možnosť Výber akcie pre neznáme potenciálne škodlivé URL adresy v správach.**
     - Vyberte **položku Použiť bezpečné prepojenia na správy odoslané v rámci organizácie**.

  Ďalšie informácie nájdete v téme [Nastavenie Trezor prepojenia v aplikácii Microsoft Defender pre Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
