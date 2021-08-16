---
title: Riešenie problémov s nasadením certifikátu overenie klienta
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020819"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Riešenie problémov s nasadením certifikátu overenie klienta

Profily klientskych certifikátov služieb Intune NDES/SCEP a PKCS/PFX sa bežne používajú spolu s inými typmi profilov, ako napríklad Wi-Fi, VPN a e-mail, aby sa používatelia mohli overiť pri podnikových zdrojoch. Keď sú tieto typy profilu prepojené s profilom certifikátu klienta, závisia od úspešného nasadenia tohto profilu.

Počiatočné nastavenie infraštruktúry a priradená konfigurácia profilu certifikátu klienta často vyžadujú riešenie problémov. Podrobné pokyny na úspešné nastavenie konektora NDES a pokyny na riešenie problémov s cieľom určiť problémy s nasadením certifikátu nájdete v týchto téme: 

- [Konfigurácia infraštruktúry na podporu SCEP so systémom Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Prehľad riešenia problémov s profilmi certifikátov SCEP so Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Overte konfiguráciu pomocou skriptov prostredia powershell, na ktoré sa odkazuje. Ďalšie informácie nájdete v téme [Skripty na overenie konektora certifikátu intune.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Ďalšie bežné problémy**

**Pri pokuse o inštaláciu konektora certifikátu služby Intune na server konektora NDES sa zobrazí hlásenie Heslo v žiadosti o certifikát nie je možné overiť. Možno sa už používal. Získajte nové heslo na odoslanie v tejto žiadosti."**  

Toto hlásenie znamená, že musíte spustiť inštaláciu konektora certifikátu ako správca.

V niektorých prostrediach musia servery, na ktorých je spustený certifikát Intune, používať na pripojenie k službe Intune server proxy, a preto musí konektor certifikátu používať server proxy. V niektorých prípadoch konektor NDES ignoruje nakonfigurované nastavenia servera proxy a môže byť potrebné nakonfigurovať nastavenia servera proxy počas spustenia v kontexte zabezpečenia systému LocalSystem. 
 
Riešením je spustiť Internet Explorer ako SYSTEM a nakonfigurovať server proxy v IE. Po reštartovaní služby Intune Connector Connector sa konektor NDES pripojí k službe Intune.

**Používateľské zariadenia už nedoberajú certifikáty SCEP od NDES.**

Je možné, že platnosť certifikátu overenie klienta vydaného pre server NDES zadaný počas inštalácie konektora NDES uplynula alebo chýba. Riešenie: 
 
1. Odinštalujte konektor NDES.  
2. Ak chcete požiadať o nové overenie klienta alebo certifikát overovania servera, použite tieto podrobnosti: 
 
    - Názov predmetu: CN = external fqdn  
    - Alternatívny názov predmetu (oba sú povinné): DNS = external fqdn, DNS = internal fqdn 
 
3. Znova nainštalujte konektor NDES s novým certifikátom.