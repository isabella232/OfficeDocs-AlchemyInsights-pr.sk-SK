---
title: Pravidlá zmenšenia oblasti útokov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676442"
---
# <a name="attack-surface-reduction-rules"></a>Pravidlá zmenšenia oblasti útokov

Vylúčenie súborov alebo priečinkov môže vážne znížiť ochranu, ktorú poskytujú pravidlá na zníženie počtu útokov v oblasti povrchov. Súbory, ktoré by boli zablokované pravidlom, môžu byť spúšťané a nezaehrajú sa žiadne zostavy ani udalosti. Vylúčenie sa vzťahuje na všetky pravidlá, ktoré umožňujú vylúčenie.

Vylúčenia ASR používajú rovnakú syntax ako vo Microsoft Defender Antivirus vylúčenia. Podrobnosti nájdete v téme [Konfigurácia a overenie vylúčení pre Microsoft Defender Antivirus kontroly.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Ak sa chcete vyhnúť problémom, [pozrite si bežné chyby, ktorým sa vyhnete pri definovaní vylúčení](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Nie všetky pravidlá ASR podporujú vylúčenia. Ak chcete overiť, či vaše pravidlo podporuje vylúčenia, pozrite si tabuľku Pravidlá pre zníženie počtu miest útokov na [povrchu.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Pravidlá zmenšenia oblasti útokov

Útok na ploche vašej organizácie zahŕňa všetky miesta, kde útočník mohol ohroziť organizačné zariadenia alebo siete. Zníženie počtu miest útokov znamená ochranu zariadení a siete v organizácii, ktorá vnechá útoky menším spôsobom. Pomôcť môže konfigurácia pravidiel na zníženie počtu útokov v programe Microsoft Defender pre koncový bod.

Ďalšie informácie nájdete v téme:

- [Priradenie identifikátora GUID pravidla ASR k názvu](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Požiadavky pravidiel ASR:
    - [Windows 10 Pro, verzia 1709 alebo novšia](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, verzia 1709 alebo novšia](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, verzia 1803 (polročné kanály) alebo novšia](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identifikácia správneho vylúčenia, ktoré je potrebné použiť

1. V denníku eventID 1121 alebo 1122 vyhľadajte položku eventID 1122 Windows-Windows Defender/Operational.

1. Vyhodnoťte scenár blokovania a kontext a potvrďte, že tento scenár je potrebné odblokovať.

1. Prečítajte si hodnotu Cesta v podrobnostiach udalosti, čo je hodnota, ktorá definuje vylúčenie.
    - Vylúčenie vykonajte čo najprísnejšie.
    - V prípade potreby použite zástupný znak (napríklad nahraďte premennú Používateľa).

1. Vylúčenie použite podľa potrieb nasadenia. Podrobné informácie nájdete v téme [Prispôsobenie pravidiel na zníženie počtu útokov v povrchovom zariadení.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Vylúčenie nie je ocenené

1. Určite, či pravidlo podporuje vylúčenia. Podrobnosti nájdete v téme Pravidlá [na zníženie počtu povrchov útokov.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Skontrolujte použité vylúčenia a v údajoch udalosti overte preklepy alebo nesprávne použité zástupné znaky. Ďalšie informácie nájdete v téme [Podporované typy vylúčenia.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. ak je vplyv pravidla príliš vysoký, zvážte presunutie pravidla (späť) do režimu auditu a vykonanie ďalšieho overenia. Podrobnosti nájdete v téme [Testovanie funkcií Microsoft Defendera pre koncové body v režime auditu.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Zhromaždite údaje podpory na otvorenie prípadu podpory pomocou tohto príkazu:
    
   ** MDEClientAnalyzer.cmd -v**

    Ďalšie informácie nájdete v téme [Problémy s onboarding zariadeniami s aplikáciou Microsoft Defender pre koncové body.](issues-with-onboarding-machines.md)
