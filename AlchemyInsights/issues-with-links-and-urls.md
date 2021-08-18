---
title: Problémy s prepojeniami a URL adresami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321922"
---
# <a name="issues-with-links-and-urls"></a>Problémy s prepojeniami a URL adresami

URI identifikátor presmerovania/URL adresa odpovede (oba výrazy sú zameniteľné) sú URL adresy, ktoré platforma Microsoft identity platform využíva na vrátenie tokenov vyžadovaných aplikáciou. Informácie o týchto URL adresách nájdete v týchto článkoch:

- [Postupy overovania a scenáre pre aplikácie](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – Informácie o URI identifikátoroch presmerovaní na stránke **Registrácie aplikácií** pre každý scenár.
- [Obmedzenia URI identifikátora presmerovania/URL adries odpovede](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Neviem ako zaregistrovať správny URI identifikátor presmerovania/URL adresu odpovede pre moju aplikáciu**

Ak sa pri prihlásení s aplikáciou, ktorú vyvíjate, na prihlasovacom dialógovom okne zobrazí **AADSTS50011: URL adresa odpovede špecifikovaná v žiadosti sa nezhoduje s URL adresami odpovede, ktoré sú nakonfigurované pre aplikáciu. <your app ID>** Do registrácie aplikácie budete musieť pridať URI identifikátor presmerovania, ktorý váš kód použil v požiadavke o token odoslanej platforme Microsoft identity platform.

Ak chcete pridať URL adresu odpovede, prejdite na kartu **Overovanie** na stránke **registrácie aplikácie** na portáli Microsoft Azure a pridajte zápis do časti **URI identifikátory presmerovania**. Hodnota, ktorú musíte zadať, závisí od typu aplikácie, ktorú zostavujete, podľa tohto opisu:

- Pre jednostranové aplikácie a webové aplikácie je URL adresa odpovede URL adresa vo vašej aplikácii. Pozrite si tému[Registrácia jednostranovej aplikácie](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) alebo [Registrácia webovej aplikácie pomocou portálu Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Pri počítačových aplikáciách závisí hodnota, ktorú potrebujete vybrať, od:
    - platformy (MacOS sa líši od Windowsu alebo Linuxu)
    - spôsobu získavania tokenu (interaktívne, s kódom toku spracovania zariadenia, integrované overovanie systému Windows [IWA] alebo pomocou mena používateľa/hesla).
    Podrobnosti nájdete v téme [Počítačové aplikácie – URI identifikátor presmerovania](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Pri mobilných aplikáciách závisí URI identifikátor presmerovania od:
    - platformy (iOS/Android/UWP)
    - informácií využité na zostavenie aplikácie ako napríklad ID balíka v iOS, názov balíka a odtlačok hash podpisu v Androide. Registrácia aplikácie na portáli Microsoft Azure vám pomôže. Viac informácií nájdete na [Konfigurácia platformy a URI identifikátory presmerovania](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Poznámka:** Webové rozhrania API a niektoré z tichých spôsobov získania tokenov (IWA a meno používateľa/heslo) nevyžadujú identifikátor URI na presmerovanie.

**Nasadil som svoju webovú aplikáciu a keď ju testujem, zobrazí sa správa, že URL adresa odpovede sa nezhoduje**

Pridať URI identifikátory presmerovaní pre všetky lokality, na ktoré nasadzujete svoju webovú aplikáciu. Viac informácií nájdete v téme [Registrácia webovej aplikácie pomocou portálu Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Poznámka:** Identifikátor URI presmerovania môžete pridať do umiestnenia hneď po nasadení aplikácie v tomto umiestnení.

**Nemôžem zaregistrovať dostatočné množstvo URL adries odpovede**

Ste nezávislý odberateľ softvéru a máte jeden alebo niekoľko URI identifikátorov presmerovania pre každého zákazníka. Chcete migrovať z ADAL/Azure AD v1.0 na MSAL/Microsoft identity platform a dosiahli ste [maximálny počet URI identifikátorov presmerovania](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Tento problém vyriešite, keď [pridáte URI identifikátory presmerovania objektom služieb](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), ktoré sa zhodujú s každým vašim zákazníkom.
