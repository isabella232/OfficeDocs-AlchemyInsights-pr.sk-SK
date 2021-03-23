---
title: Problémy so správou používateľov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037508"
---
# <a name="user-management-issues"></a>Problémy so správou používateľov

**Čo sa stane so súčasnými priradenými používateľmi aplikácie, ak vypnem Vlastnosť User priradenia (nastavte túto vlastnosť na možnosť nie)?**

Vypnutie **povinného nasadenia používateľa** nemá vplyv na aktuálne priradených používateľov. Vypnutie tejto vlastnosti umožní všetkým používateľom prístup k aplikácii. Všetci uvedení používatelia a používatelia, ktorí sú priradení k skupinám v aplikácii, budú naďalej platné.

- Ak chcete obmedziť svoju aplikáciu na konkrétnu skupinu používateľov, prečítajte si tému – [obmedzenie aplikácie Azure AD na množinu používateľov – platforma Microsoft Identity | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Ak chcete priradiť používateľov a skupiny k podnikovým aplikáciám v službe Azure Active Directory (Azure AD), a to buď z portálu Azure alebo pomocou prostredia PowerShell, pozrite si tému [Správa používateľských priradení aplikácie v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Ak chcete delegovať povolenia na vytváranie a správu aplikácií, pozrite si tému [povolenia správcu spravovania aplikácií – Azure AD | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Skrytie konkrétnych podnikových aplikácií od používateľov** – Ak chcete skryť všetky aplikácie Microsoft 365 z panela **aplikácie** , použite nasledujúci postup. Aplikácie sa budú aj naďalej zobrazovať na portáli Office 365.

 1. Prihláste sa na portáli Azure ako globálny správca vášho adresára. 
 2. Vyberte položku **Azure Active Directory**. 
 3. Vyberte položku **Používatelia**. 
 4. Vyberte položku **nastavenia používateľa**. 
 5. V časti **podnikové aplikácie** kliknite na položku **Spravovať spôsob spúšťania a zobrazovania aplikácií koncovými používateľmi**. 
 6. **Používatelia môžu v portáli office 365 Zobraziť len aplikácie balíka office 365**, kliknite na tlačidlo **Áno**. 
 7. Kliknite na tlačidlo **Uložiť**. 
 8. Ďalšie informácie nájdete v téme [skrytie podnikovej aplikácie zo skúseností používateľov v službe Azure AD | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Ak ponúkate softvér ako aplikáciu služby (SaaS) viacerým organizáciám, môžete svoju aplikáciu nakonfigurovať tak, aby prijímala prihlasovacie moduly z ľubovoľného nájomníka služieb Azure Active Directory (Azure AD). Táto konfigurácia sa nazýva "sprístupnenie viacerých nájomníkov aplikácie". Používatelia v ľubovoľnom nájomníkovi služby Azure AD sa budú môcť prihlásiť do aplikácie po súhlase s používaním svojho konta v aplikácii. Ďalšie informácie nájdete v téme [vytváranie aplikácií, ktoré sa prihlasujú v Azure AD Users – Microsoft Identity Platform | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Ako môže koncový používateľ získať prístup k aplikácii po priradení k žiadosti?**

Každá aplikácia v Blade podnikovej aplikácie obsahuje prepojenie na koncových používateľov, ktorí majú prístup. Používatelia budú môcť jednoducho získať prístup k aplikácii prostredníctvom portálu **aplikácie** .

- **Chcete vedieť, ktoré aplikácie a typ aplikácií používajú používatelia?**

Správy o prihlasovaní si môžete stiahnuť za posledných 30 dní od **portal.azure.com > Azure Active directory> Signins> download Reports**.

- Získajte informácie o tom, ako [udeliť súhlas súhlasu správcu pre aplikáciu](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) a [Nakonfigurujte spôsob súhlasu koncových používateľov na aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Oboznámte sa s tým, [ako funguje súhlas](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) a [spravuje súhlas s aplikáciami](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


