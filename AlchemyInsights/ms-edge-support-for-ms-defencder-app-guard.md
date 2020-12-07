---
title: Microsoft Edge Support pre aplikáciu Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584011"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge Support pre aplikáciu Microsoft Defender Application Guard

Aplikácia Guard je navrhnutá pre Windows 10 a Microsoft Edge, ktorá používa hardvérový izolačný prístup, ktorý umožňuje používateľovi prejsť na nedôveryhodnú lokalitu zvnútra izolovaného, Hyper-V-povoleného kontajnera oddeleného od hostiteľského operačného systému.

Podnikový správca definuje zoznam dôveryhodných webových lokalít, cloudových zdrojov a interných sietí. Keď používateľ navštívi lokalitu, ktorá sa nenachádza v zozname, Microsoft Edge otvorí lokalitu v kontajneri. To znamená, že ak sa lokalita ukáže ako škodlivá, hostiteľský počítač zostane zabezpečený a útočník sa nedostane do podnikových údajov.

Inštalácia rozšírení v kontajneri je podporovaná v prehliadači Microsoft Edge verzie 81 a môže byť riadená prostredníctvom politiky. Adresa updateURL, ktorá sa použije v politike ExtensionInstallForcelist, by sa mala pridať ako neutrálny zdroj v politike izolácie siete, ktorú používa strážca aplikácie.

Ďalšie informácie nájdete v téme [podpora aplikácie Microsoft Edge pre aplikáciu Microsoft Defender Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
