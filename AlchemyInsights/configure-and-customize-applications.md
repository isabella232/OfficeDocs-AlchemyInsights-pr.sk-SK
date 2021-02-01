---
title: Konfigurácia a prispôsobenie aplikácií
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063665"
---
# <a name="configure-and-customize-applications"></a>Konfigurácia a prispôsobenie aplikácií

**Konfigurácia aplikácií**

1. [QuickStart: Konfigurácia vlastností aplikácie v nájomníkovi služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vám ukáže, ako nakonfigurovať niektoré vlastnosti aplikácie.
2. Na pomoc pri integrácii aplikácií pomocou služby Azure Active Directory sme vytvorili [kolekciu kurzov](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) , ktoré vás prevedie konfiguráciou.
3. [Konfigurovanie aplikácie proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) aplikácie vám pomôže pochopiť, ako nakonfigurovať aplikáciu proxy aplikácie v rámci služby Azure AD na odhalenie lokálnych aplikácií do cloudu.
4. [Stiahnuť PingAccess a nakonfigurovať aplikáciu](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): postupujte podľa pokynov v *téme Konfigurácia PINGACCESS pre Azure AD na ochranu aplikácií* publikovaných pomocou servera proxy aplikácie Microsoft Azure AD na webovej lokalite služby ping identity a Stiahnite si najnovšiu verziu programu PingAccess.

**Nesprávne nakonfigurované chyby aplikácie (AADSTS650056)**

1. Uistite sa, že pristupujete k aplikácii z prihlasovacej adresy, ktorú vám poskytol vlastník aplikácie. V opačnom zmysle sa prihláste do aplikácie prostredníctvom normálneho procesu. Vo väčšine prípadov sa táto funkcia automaticky vyrieši prirodzene. Ak to tak nie je, tento príspevok môže pomôcť pri riešení problémov a riešení tohto problému.
2. **Ak vaša organizácia vlastní aplikáciu** (čo znamená, že registrácia aplikácie je vo vašej organizácii):
    - Na minimum odporúčame, aby sa `User.Read` pridal alebo `openid` delegované povolenie z **Microsoft Graphu** .
    - Uistite sa, že aplikácia a všetky jej povolenia súhlasia. Môžete to overiť tak, že sa pozriete na stĺpec **stav** v časti registrácia aplikácie v rámci **povolení rozhrania API**.
    - V niektorých prípadoch môže byť aplikácia treťou stranou, avšak môže byť zaregistrovaná vo vašej organizácii. Potvrďte, či je táto aplikácia uvedená v žiadostiach o registráciu aplikácie (nie podnikové aplikácie).
    - Ak sa toto chybové hlásenie zobrazuje aj naďalej. Potom možno bude potrebné vytvoriť URL adresu súhlasu opísanú v **kroku 4**.
3. **Ak vaša organizácia nie je vlastníkom aplikácie a používate ju ako aplikáciu tretej strany**:
    - Ak ste globálnym/firemným správcom, mali by ste vidieť obrazovku s súhlasu. Uistite sa, že začiarknete políčko **"súhlas v mene vašej organizácie"**.
    - Ak sa nezobrazuje obrazovka súhlas, odstráňte podnikovú aplikáciu a skúste to znova.
    - Ak sa toto chybové hlásenie zobrazuje aj naďalej. Potom možno bude potrebné vytvoriť URL adresu súhlasu opísanú v **kroku 4**.
4. **Manuálne vytvorenie URL adresy súhlasu, ktorá sa má použiť**: Ak je aplikácia navrhnutá na prístup k určitému zdroju, pravdepodobne nebudete môcť použiť tlačidlá súhlasu z portálu Azure, budete musieť manuálne vytvoriť URL adresu s vlastným súhlasom a použiť ju.
    - Budete musieť získať `{App-Id}` a `{App-Uri-Id}` od vlastníka aplikácie. `{Tenant-Id}` bude identifikátor nájomníka. Bude to buď `yourdomain.onmicrosoft.com` ID vášho adresára.
    - Ak sa v rámci aplikácie pristupuje k zdroju, potom `{App-Id}` `{App-Uri-Id}` bude rovnaká.
5. Ďalšie informácie nájdete v téme [problémy s prihlasovaním do jediného prihlásenia založeného na SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Prispôsobenie aplikácií**

- [Pridanie značky na prihlasovaciu stránku v službe Azure Active Directory vašej organizácie](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – použite logo vašej organizácie a vlastné farebné schémy, ktoré vám poskytnú konzistentný vzhľad na prihlasovacej stránke služby Azure Active Directory (Azure AD).
- [Pridanie vlastného názvu domény pomocou portálu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – každý nový nájomník služby Azure AD sa dodáva s počiatočným názvom domény. Pôvodný názov domény nie je možné zmeniť ani odstrániť, ale môžete pridať mená svojej organizácie. Pridanie vlastných názvov domén vám pomôže vytvoriť mená používateľov, ktoré sú známe vašim používateľom.
