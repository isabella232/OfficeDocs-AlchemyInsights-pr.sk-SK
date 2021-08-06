---
title: Password Writeback is not working
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999759"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback is not working

**Mám problémy s konfiguráciou funkcie WriteBack pre heslo**

- Funkcia Password writeback je prémiová funkcia.
- Uistite sa, že rozumiete licenčným požiadavkám:
  - Musíte mať vo svojej organizácii priradenú aspoň jednu licenciu
  - **Len používatelia v cloude** – všetky Office 365 (O365) platené SKU alebo Azure AD Basic
  - **Cloud a/alebo** lokálni používatelia – Azure AD Premium P1 alebo P2, Enterprise Mobility + Security (EMS) alebo Secure Productive Enterprise (SPE)
    - Ďalšie informácie o licenčných požiadavkách nájdete v téme [Licenčné požiadavky na samoobslužné vytvorenie nového](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) hesla pre Azure AD.
- Máte aspoň jedno konto správcu a jedno skúšobné používateľské konto s jednou z príslušných licencií.
- Ak chcete, aby funguje služba writeback hesla Pripojenie Azure AD Pripojenie k primárnemu emulátorovi radiča domény. Azure AD Pripojenie môžete nakonfigurovať na používanie primárneho radiča  domény kliknutím pravým tlačidlom myši na vlastnosti konektora synchronizácie služby Active Directory a výberom položky Konfigurovať oblasti **adresára.** Tu vyhľadajte časť s nastaveniami **pripojenia radiča** domény a začiarknite políčko s názvom **Používať iba preferované radiče domén.**
  > [!NOTE]
  > Ak preferované DC nie je emulátor PDC, Azure AD Pripojenie bude aj naďalej kontaktovať službu PDC na zápis hesla.
- V nájomníkovi bolo nakonfigurované a povolené vytvorenie nového hesla. Ďalšie informácie nájdete v téme [Povolenie používateľom obnoviť heslá v službe Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Skontrolujte, či konto správcu používané na povolenie funkcie Password Writeback je konto správcu cloudu (vytvorené v Azure AD nie v lokálnej službe AD)
- Máte jedno alebo viac doménové nasadenie AD spustené Windows Server 2008 R2, Windows Server 2012 alebo Windows Server 2012 R2 s nainštalovanými najnovšími balíkmi Service Pack
- Máte nainštalovaný nástroj Azure AD Pripojenie a pripravili ste prostredie AD na synchronizáciu do cloudu. Pred testovaním funkcie writeback hesiel skontrolujte, či ste najprv dokončili úplnú synchronizáciu importu a úplnej synchronizácie zo služby AD a Azure AD v službe Azure AD Pripojenie.
- Ďalšie informácie nájdete v téme Postup úplnej synchronizácie a [úplného importu v službe Azure AD Pripojenie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Mám problém s pripojiteľnosťou funkcie WriteBack pre heslo**

1. Stiahnite si a povoľte najnovšiu [verziu služby Azure AD Pripojenie](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfigurácia brány firewall: Nástroj Azure AD Pripojenie (1.1.443 a novší) bude potrebovať prístup **HTTPS** odchádzajúcich údajov na:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Povolenie nečinnosti pripojení pretrvajú minimálne 2 – 3 minúty

**Stále sa mi nená pomýlili problémy s písaním hesla**

- Ak problémy aj naďalej pretrváva, skúste vypnúť a znova zapnúť službu zapisovania hesiel v nástroji Azure AD Pripojenie.
- Ďalšie informácie nájdete v téme Ako [vypnúť a znova zapnúť funkciu writeback hesla.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
