---
title: Problémy s prepojeniami a URL adresami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974753"
---
# <a name="issues-with-links-and-urls"></a>Problémy s prepojeniami a URL adresami

Presmerovanie URL adries URI a odpovedí (obidva výrazy sú zameniteľné) sú URL adresy, ktoré používa platforma Microsoft identity na vrátenie tokenov vyžadovaných aplikáciou. Informácie o týchto URL adresách nájdete v nasledujúcich článkoch:

- [Toky overovania a scenáre aplikácie](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informácie o presmerovaní URI na stránke **registrácia aplikácie** pre každý scenár.
- [Presmerovanie obmedzení a obmedzení URL adries URI a odpovedí](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Neviem, ako sa zaregistrovať správne presmerovanie URL adresy URI alebo odpovede pre aplikáciu**

Keď sa prihlásite s aplikáciou, ktorú vytvárate, ak sa dialógové okno prihlásenia zobrazí **AADSTS50011: URL adresa odpovede zadaná v požiadavke sa nezhoduje s URL adresami odpovedí konfigurovanými pre danú <your app ID> aplikáciu**, budete musieť pridať do registrácie aplikácie, identifikátor URI presmerovania, ktorý používa kód v požiadavke tokenu na platformu identity spoločnosti Microsoft.

Ak chcete pridať URL adresu odpovede, prejdite na kartu **overenie** na stránke **registrácia aplikácie** na portáli Azure a pridajte položku do časti **presmerovanie URI** . Presmerovanie URI je zadané (web alebo mobil/počítač). Hodnota, ktorú treba zadať, závisí od typu aplikácie, ktorú staviate, ako je popísané nižšie:

- V prípade aplikácií s jednou stranou a webových aplikácií je URL adresa URL ADRESou v aplikácii. Pozrite si tému [registrácia aplikácie na jednu stranu](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) alebo registrácia [aplikácie webových aplikácií pomocou služby Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Ak ide o počítačové aplikácie, hodnota, ktorú treba vybrať, závisí od:
    - platforma (MacOS sa líši od Windowsu alebo Linuxu)
    - spôsob získania tokenu (interaktívne s tokom kódu zariadenia s integrovaným overovaním systému Windows [IWA] alebo s používateľským menom a heslom).
    Podrobnosti nájdete v téme [počítačové aplikácie – registrácia aplikácie – presmerovanie URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Pre mobilné aplikácie závisí URI presmerovania:
    - platforma (iOS/Android/UWP)
    - informácie, ktoré sa používajú na zostavenie aplikácie, ako je napríklad ID balíka v systéme iOS, a názov balíka a hash podpisu v Androide, ktoré vám pomôžu pri registrácii aplikácie Azure Portal. Podrobnosti nájdete v téme [Konfigurácia platformy a presmerovanie URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Webové rozhrania API a niektoré tiché spôsoby získania tokenov (IWA a meno používateľa a heslo) nevyžadujú identifikátor URI presmerovania.

**Mám nasadené webovú aplikáciu a pri testovaní nasadenej aplikácie sa zobrazí hlásenie o nezhode URL adresy odpovedí**

Pridajte presmerovanie URI pre všetky umiestnenia, v ktorých Nasadzujete webovú aplikáciu. Ďalšie informácie nájdete v téme [registrácia aplikácie webových aplikácií pomocou služby Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Pridať identifikátor URI presmerovania pre miesto ihneď po nasadení aplikácie v danom umiestnení.

**Nemôžem sa zaregistrovať dostatok URL odpovedí**

Ste ISV a máte jednu alebo viacero presmerovať URI pre každého zákazníka. Chcete migrovať z ADAL/Azure AD v 1.0 na MSAL/platformu Microsoft identity a stlačíte [maximálny počet presmerovaní URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Ak chcete tento problém vyriešiť, [Pridajte presmerovanie URI na servisné princípy](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , ktoré zodpovedajú každému zákazníkovi.
