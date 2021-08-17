---
title: Vyhľadanie chýbajúcich aplikácií na registračných číslach aplikácií
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057117"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Vyhľadanie chýbajúcich aplikácií na registračných číslach aplikácií

1. Na portáli na registráciu aplikácií sa nedajú nájsť aplikácie.

    Ak je aplikácia s viacerými nájomníkmi a bola zaregistrovaná v inom nájomníkovi, nezobrazí sa v časti Registrácia aplikácie blade. Po prístupe k aplikácii Enterprise Applications (po súhlase) ju však možno nájdete na serveri Enterprise Applications blade a v nájomníkovi sa vytvoril hlavný názov služby. Ďalšie informácie nájdete v téme [Hlavné & aplikácií v Azure AD – Microsoft identity platform.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. V programe App Registration blade sa nedajú zobrazovať aplikácie, aj keď ste správcom.

    Skontrolujte, či ste na portáli Azure v správnom adresári.
3. Moja aplikácia nie je uvedená v časti Enterprise Applications blade, ale zobrazí sa pri dotaze príkazu v prostredí PowerShell.

    Niekedy sa po odstránení aplikácie z portálu Azure aplikácia na portáli nevy zobrazí, ale možno nebola úplne odstránená. Ďalšie informácie nájdete v téme:
    - Môžete načítať zoznam predtým odstránených aplikácií a pomocou príkazu prostredia Powershell zistiť, či sa aplikácia v zozname zobrazuje: **Get-AzureADDeletedApplication.** Ďalšie informácie nájdete v [téme Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Ak chcete aplikáciu úplne odstrániť, môžete skúsiť nasledovné v prostredí PowerShell: **Remove-AzureADApplication -ObjectId.** Ďalšie informácie nájdete v téme [Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Prípadne môžete skúsiť obnoviť odstránenú aplikáciu pomocou tohto príkazu prostredia PowerShell: **Obnoviť AzureADDeletedApplication -ObjectId.** Ďalšie informácie nájdete v [téme Obnovenie AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. V mojom novom nájomníkovi Azure neviem nájsť zoznam všetkých predinštalových podnikových aplikácií.

    V službe Azure AD nie sú predvolene nainštalované žiadne predinštalné podnikové aplikácie. Budete ho musieť pridať manuálne z možnosti Nová aplikácia jej vy prehľadávaním z galérie Azure AD alebo pridaním aplikácie, ktorá nie je z galérie. Ďalšie informácie nájdete v téme [Rýchly štart: Pridanie aplikácie do nájomníka služby Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Ak ste globálnym správcom, môžete jednoducho pristupovať k aplikáciám pomocou [spúšťača Microsoft 365 aplikácií](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Nepodarilo sa nájsť moje aplikácie z portálu Moje aplikácie.

    Uistite sa, že aplikácie nie sú na stránke kolekcie Moje aplikácie skryté. Ďalšie informácie nájdete v téme [Kolekcie (ukážka) na portáli Moje aplikácie – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Ak chcete spustiť aplikácie z portálu Moje aplikácie, pozrite si & Vyhľadanie a používanie [aplikácií na portáli Moje aplikácie – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Aplikácia Mover sa po inštalácii nezobrazuje na serveri Enterprise Applications blade.

    Aplikácia Office 365 Mover je aplikácia s viacerými nájomníkmi, ktorú nie je potrebné pridať do služby AAD pomocou časti Aplikácie galérie v rámci registrácie podnikovej aplikácie. Ak chcete Office 365 aplikáciu Mover, jednoducho sa prihláste do aplikácie a vyžaduje od používateľa súhlas na získanie povolení. Keď používateľ poskytne súhlas, táto aplikácia sa automaticky pridá do nájomníka s e-mailovým ID, ktoré ste sa prihlásili.

    Po prihlásení do aplikácie by malo byť možné vyhľadať záznam tejto aplikácie v rámci bladeu podnikových aplikácií v AAD. Túto aplikáciu musíte vyhľadať zadaním celého mena, t. j. slovné Office 365 Mover alebo jednoducho pomocou vyhľadávania "office", kde by sa mala nachádzať zoznam aplikácie. Ďalšie informácie nájdete v Office 365, že premiestňovanie je už nainštalované, ale nie je uvedený v [galérii podnikových aplikácií.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Rýchly štart: V zobrazení zoznamu aplikácií, ktoré používajú vášho nájomníka [služieb Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) na spravovanie identít, sa zobrazí postup na zobrazenie aplikácií, známych aj ako aplikácie, ktoré sú už nastavené na používanie nájomníka služby Azure AD ako poskytovateľa identity (IdP).
9. [Riešenie bežných problémov s pridávaním alebo odstraňovaním](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) aplikácie v Azure Active Directory pomáha pochopiť bežné problémy, ktorým ľudia pri prezeraní aplikácií Azure Active Directory.
