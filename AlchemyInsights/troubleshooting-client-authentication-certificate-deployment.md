---
title: Riešenie problémov s nasadením certifikátu overenia klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555810"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Riešenie problémov s nasadením certifikátu overenia klienta

Intune NDES/SCEP a PKCS/PFX klientske certifikáty profily sa bežne používajú v spojení s inými typmi profilov, ako je Wifi, VPN a e-mail, aby používatelia mohli overiť podnikové zdroje. Keď tieto typy profilov sú prepojené s profilom certifikátu klienta sú závislé na úspešné nasadenie tohto profilu.

Počiatočné nastavenie infraštruktúry a súvisiace konfigurácie profilu certifikátu klienta často vyžadujú riešenie problémov. Podrobný sprievodca úspešné nastavenie konektora NDES a pokyny na riešenie problémov na izoláciu problémov s nasadením certifikátu nájdete na: 

- [Konfigurácia infraštruktúry na podporu protokolu SCEP s intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Prehľad problémov s profilmi certifikátov SCEP s Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Na overenie konfigurácie použite odkazované skripty prostredia PowerShell. Ďalšie informácie nájdete v téme [Skripty na overenie konektora certifikátu intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Ďalšie bežné otázky**

**Pri pokuse o inštaláciu konektora certifikátu Intune na konektor NDES server, dostanem správu, "heslo v žiadosti o certifikát nie je možné overiť. To môže byť použitý už. Získať nové heslo na odoslanie s touto požiadavkou."**  

Toto hlásenie znamená, že musíte spustiť inštaláciu konektora certifikátu ako správca.

V niektorých prostrediach servery, kde je spustený certifikát Intune, musia na pripojenie k intune použiť server proxy, a preto musí certifikačná konzola používať server proxy. V niektorých prípadoch NDES konektor ignoruje nakonfigurovaný nastavenia servera proxy a môže byť potrebné nakonfigurovať nastavenia servera proxy pri spustení v kontexte zabezpečenia LocalSystem. 
 
Riešením je spustiť program Internet Explorer ako systém a nakonfigurovať proxy v IE. Po reštarte služby Konektor Intune, Konektor NDES sa pripojí k Intune.

**Používateľské zariadenia už nedostávajú certifikáty SCEP z NDES.**

Je možné, že certifikát overenia klienta vydaný na server NDES a zadaný počas inštalácie konektora NDES uplynula alebo chýba. Riešenie: 
 
1. Odinštalovať konektor NDES.  
2. Tieto podrobnosti použite na vyžiadanie nového certifikátu overenia klienta alebo servera: 
 
    - Názov predmetu: CN = externý fqdn  
    - Alternatívny názov predmetu (obe sú povinné): DNS = externé fqdn, DNS = interné fqdn 
 
3. Preinštalujte konektor NDES s novým certifikátom.