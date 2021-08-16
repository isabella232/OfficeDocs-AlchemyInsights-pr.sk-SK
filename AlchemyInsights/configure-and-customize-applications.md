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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045003"
---
# <a name="configure-and-customize-applications"></a>Konfigurácia a prispôsobenie aplikácií

**Konfigurovanie aplikácií**

1. [Rýchly štart: Konfigurácia vlastností aplikácie v nájomníkovi služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vám ukáže, ako konfigurovať niektoré vlastnosti aplikácie.
2. S cieľom integrovať vaše aplikácie so servermi Azure Active Directory sme vytvorili [kolekciu](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) kurzov, ktoré vás presťujú konfiguráciou.
3. [Postup konfigurácie aplikácie proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) vám pomôže pochopiť, ako nakonfigurovať aplikáciu proxy aplikácie v Azure AD, aby sa vaše lokálne aplikácie vystavili cloudu.
4. [Stiahnite si PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)Microsoft Azure AD nakonfigurujte aplikáciu: Postupujte podľa pokynov v článku Konfigurácia *pingAccess* pre Azure AD na ochranu aplikácií publikovaných pomocou proxy aplikácie na webovej lokalite Ping Identity Microsoft Azure AD stiahnite si najnovšiu verziu príkazu PingAccess.

**Chyby nesprávne nakonfigurovanej aplikácie (AADSTS650056)**

1. Uistite sa, že k aplikácii pristupuje z prihlasovacej adresy, ktorú vám poskytol vlastník aplikácie. V opačnom prípade sa prihláste do aplikácie bežným spôsobom. Vo väčšine prípadov sa to automaticky vyrieši prirodzene. Ak sa tak stane, tento príspevok vám pomôže pri riešení problémov a riešení.
2. **Ak je aplikácia vo vašom vlastníctve vašej organizácie** (čo znamená, že registrácia aplikácie je vo vašej organizácii):
    - Odporúčame minimálne pridať alebo `User.Read` delegovaný prístup `openid` od spoločnosti Microsoft **Graph** pridávať.
    - Uistite sa, že aplikácia a všetky jej povolenia sú so súhlasom. Môžete to overiť tak, že si **prezeráte** stĺpec Stav registrácie aplikácie v rámci povolení **API.**
    - V niektorých prípadoch môže byť aplikácia treťou stranou, ale môže byť zaregistrovaná vo vašej organizácii. Potvrďte, či je táto aplikácia uvedená v registráciách aplikácií (nie aplikácie Enterprise).
    - Ak sa toto chybové hlásenie zobrazuje aj naďalej. Potom možno budete musieť zostaviť URL adresu súhlasu, ktorá je popísaná v **kroku 4.**
3. **Ak vaša organizácia nie je vlastníkom aplikácie a používa ju ako aplikáciu tretej strany:**
    - Ak ste správcom spoločnosti Global/Company, mala by sa vám zobraziť obrazovka so súhlasom. Uistite sa, že začiarknete **políčko "Súhlas v mene vašej organizácie".**
    - Ak sa obrazovka so súhlasom zobraziť, odstráňte aplikáciu Enterprise a skúste to znova.
    - Ak sa toto chybové hlásenie zobrazuje aj naďalej. Potom možno budete musieť zostaviť URL adresu súhlasu, ktorá je popísaná v **kroku 4.**
4. Manuálne si vytvorte **URL** adresu súhlasu, ktorá sa má použiť: Ak je aplikácia navrhnutá na prístup ku konkrétnemu zdroju, možno nebudete môcť použiť tlačidlá Súhlas z portálu Azure, budete musieť manuálne vygenerovať svoju VLASTNÚ URL adresu súhlasu a použiť ju.
    - Budete musieť získať a `{App-Id}` od `{App-Uri-Id}` vlastníka aplikácie. `{Tenant-Id}` bude vaším identifikátorom nájomníka. Buď, alebo `yourdomain.onmicrosoft.com` ID vášho adresára.
    - Ak aplikácia používa pre zdroj samotný prístup, potom `{App-Id}` bude `{App-Uri-Id}` rovnaký.
5. Ďalšie informácie nájdete v téme Problémy s prihlásením do aplikácií s konfiguráciou jediného prihlásenia na [základe saML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Prispôsobenie aplikácií**

- [Pridanie](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) značky na prihlasovaciu stránku organizácie Azure Active Directory – použite logo organizácie a vlastné farebné schémy a dodáte tak prihlasovacím stránkam Azure Active Directory (Azure AD) jednotný vzhľad Azure Active Directory (Azure AD).
- [Pridajte vlastný názov domény pomocou portálu Azure Active Directory –](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) každý nový nájomník služby Azure AD má počiatočný názov domény. Počiatočný názov domény nie je možné zmeniť ani odstrániť, môžete však pridať názvy organizácie. Pridanie vlastných názvov domén vám pomôže vytvoriť mená používateľov, ktoré sú známe používateľom.
