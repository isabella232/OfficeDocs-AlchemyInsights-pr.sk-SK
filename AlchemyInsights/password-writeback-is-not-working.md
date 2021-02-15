---
title: Heslo zápisom nefunguje
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243522"
---
# <a name="password-writeback-is-not-working"></a>Heslo zápisom nefunguje

**Mám problémy s konfiguráciou hesla zápisom**

- Funkcia Password zápisom je prémiovou funkciou.
- Uistite sa, že chápete licenčné požiadavky:
  - V organizácii musíte mať priradenú aspoň jednu licenciu.
  - **Iba používatelia cloudu** – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic
  - **Cloudové a/alebo lokálne používatelia** – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)
    - Ďalšie informácie o licenčných požiadavkách nájdete [v téme licenčné požiadavky na vytvorenie nového hesla služby Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Máte aspoň jedno konto správcu a jedno skúšobné používateľské konto s jednou z príslušných licencií.
- Pripojenie Azure AD sa musí pripojiť k primárnemu emulátoru radiča domény na zápisom hesla. Azure AD Connect môžete nakonfigurovať tak, aby používal primárny radič domény kliknutím pravým tlačidlom myši na **Vlastnosti** konektora synchronizácie služby Active Directory a potom vyberte položku **konfigurovať oblasti adresárov**. Pozrite si časť **Nastavenie pripojenia radiča domény** a začiarknite políčko s názvom **iba preferované radiče domén**.
  > [!NOTE]
  > Ak prednostné DC nie je emulátorom PDC, Azure AD Connect bude stále osloviť PDC pre heslo zápisom.
- Obnovenie hesla bolo nakonfigurované a povolené v nájomníkovi. Ďalšie informácie nájdete v téme [Povolenie používateľom obnoviť svoje heslá v službe Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Uistite sa, že konto správcu používané na povolenie hesla zápisom je kontom správcu cloudu (vytvorené v službe Azure AD nie lokálneho AD)
- Máte jedno alebo viaceré lesné AD lokálne nasadenie so systémom Windows Server 2008 R2, Windows Server 2012 alebo Windows Server 2012 R2 s nainštalovanými najnovšími balíkmi Service Pack
- Máte nainštalovaný nástroj Azure AD Connect a máte pripravené prostredie na synchronizáciu v cloude. Pred vykonaním testovania hesla zápisom Skontrolujte, či ste najprv dokončili úplný import a úplnú synchronizáciu zo služby AD a Azure AD v službe Azure AD Connect.
- Ďalšie informácie nájdete v téme postup pri [úplnej synchronizácii a úplnom importovaní v službe Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Mám problém s pripojením hesla zápisom**

1. Stiahnutie a povolenie najnovšej verzie služby [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfigurácia brány firewall: nástroj Azure AD Connect (1.1.443 a novší) bude potrebovať **ODCHÁDZAJÚCE https** prístup k:
    - passwordreset.microsoftonline.com
    - ServiceBus. Windows. Networks
3. Povolenie nečinných pripojení trvá minimálne 2-3 minút

**Stále mám problémy s heslom zápisom**

- Ak problémy pretrvávajú, skúste vypnúť a znova zapnúť službu Password zápisom v nástroji Azure AD Connect
- Ďalšie informácie nájdete v téme [Vypnutie a opätovné zapnutie hesla zápisom](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
