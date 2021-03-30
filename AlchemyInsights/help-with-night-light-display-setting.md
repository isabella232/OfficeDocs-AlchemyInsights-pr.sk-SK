---
title: Pomoc s nastavením nočného osvetlenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405180"
---
# <a name="help-with-the-night-light-display-setting"></a>Pomoc s nastavením nočného osvetlenia

Ďalšie informácie o nastaveniach nočného času zobrazenia nájdete v [téme Nastavenie nočného času obrazovky vo Windowse 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Ak sú možnosti nočného osvetlenia v nastaveniach sivé, skontrolujte ovládač obrazovky: 

1. Kliknite na vyhľadávacie pole na paneli úloh a zadajte výraz **Správca** zariadení a potom vo **výsledkoch hľadania** vyberte položku Správca zariadení.
1. Rozbaľte **položku Display adapters (Zobrazovacie adaptéry).** 

Funkcia nočného osvetlenia však nie je k dispozícii, ak vaše zariadenie používa ovládač DisplayLink alebo ovládač základného zobrazenia.

Funkcia nočného osvetlenia využíva najnovšie grafické technológie, preto môže byť potrebné aktualizovať ovládač obrazovky:  

- Ak chcete vyhľadať aktualizácie, vyberte **položky**  >  **Nastavenie aktualizácie**&  >  **Zabezpečenie** Služby Windows  >  **Update**  >  **Vyhľadať aktualizácie.**  

ALEBO

- Ak chcete manuálne stiahnuť a nainštalovať najnovšie ovládače obrazovky, navštívte webovú lokalitu podpory výrobcu hardvéru.

## <a name="reset-night-light-in-the-registry"></a>Resetovanie nočného osvetlenia v databáze Registry

Ak aktualizácia ovládača obrazovky nefunguje, možno bude v databáze Registry potrebné obnoviť nočné osvetlenie.  

**Upozornenie:** Tento krok riešenia problémov sa odporúča iba pre pokročilých používateľov. Ak databázu Registry upravíte nesprávne, môžu sa vyskytnúť závažné problémy. Na ešte pridanú ochranu si databázu Registry pred úpravou zálohujte, aby ste ju v prípade problémov mohli obnoviť.

1. Do vyhľadávacieho poľa zadajte príkaz **regedit** a potom vo výsledkoch hľadania vyberte položku **Editor** databázy Registry.

1. Prejdite na nasledujúci kľúč databázy Registry: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Export a potom odstráňte nasledujúci podkľúč:$$windows.data.bluelightreduction.bluelightreductionstate

1. Export a potom odstráňte nasledujúci podkľúč:$$windows.data.bluelightreduction.settings

1. Reštartujte Windows a overte, či sú k dispozícii možnosti nočného osvetlenia.


