---
title: Riešenie problémov s nasadením certifikátu overenia klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659001"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Riešenie problémov s nasadením certifikátu overenia klienta

Profily klientskych certifikátov služby Intune NDES/SCEP a PKCS/PFX sa bežne používajú v spojení s inými typmi profilov, ako je napríklad WiFi, VPN a e-mailom, aby mohli používatelia autentifikovať podnikové zdroje. Keď sú tieto typy profilu prepojené s profilom certifikátu klienta, závisia od úspešného nasadenia daného profilu.

Nastavenie počiatočnej infraštruktúry a súvisiaca Konfigurácia profilu certifikátu klienta často vyžadujú riešenie problémov. Podrobný návod na úspešné Nastavenie konektora NDES a pokyny na riešenie problémov na izolovanie problémov s nasadením certifikátu nájdete v témach: 

- [Konfigurácia infraštruktúry na podporu protokolu SCEP so službou Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Prehľad na riešenie problémov s profilmi certifikátu protokolu SCEP so službou Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Na overenie konfigurácie použite odkazové skripty prostredia PowerShell. Ďalšie informácie nájdete v téme [skripty na overenie konektora služby Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Ďalšie bežné problémy**

**Pri pokuse o inštaláciu konektora certifikátu Intune na serveri konektora NDES sa zobrazí hlásenie "heslo v žiadosti o certifikát nie je možné overiť. Môže sa použiť už. Získajte nové heslo na odoslanie s touto požiadavkou.**  

Toto hlásenie znamená, že je potrebné spustiť inštaláciu konektora certifikátu ako správca.

V niektorých prostrediach musia servery, v ktorých sa spustí certifikát služby Intune, použiť server proxy na pripojenie k službe Intune, a preto musí konektor certifikátu použiť server proxy. V niektorých prípadoch NDES spojnica ignoruje nakonfigurované nastavenia servera proxy a pri spustení v kontexte zabezpečenia funkcie LocalSystem môže byť potrebné nakonfigurovať nastavenia servera proxy. 
 
Riešením je spustiť Internet Explorer ako systém a nakonfigurovať server proxy v programe IE. Po reštartovaní služby Intune Connector sa konektor NDES pripojí k službe Intune.

**Používateľské zariadenia už neprijímajú certifikáty SCEP z NDES.**

Je možné, že certifikát klientskeho overenia vydaný na server NDES a zadaný počas inštalácie konektora NDES uplynul alebo chýba. Ak chcete vyriešiť: 
 
1. Odinštalujte konektor NDES.  
2. Pomocou týchto podrobností si môžete vyžiadať nový certifikát overenia klienta alebo overenie servera: 
 
    - Názov predmetu: CN = external FQDN  
    - Alternatívny názov predmetu (vyžaduje sa oboje): DNS = externý FQDN, DNS = Internal FQDN 
 
3. Preinštalujte konektor NDES s novým certifikátom.