---
title: Odstrániť nájomníka
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993908"
---
# <a name="delete-tenant"></a>Odstrániť nájomníka

Ak chcete odstrániť Azure AD, uistite sa, že:
- Ste globálnym správcom adresára.
- NIE ste prihlásení pomocou konta, ktoré má predvolený adresár, ako je napríklad contoso.onmicrosoft.com v podpísanom konte, napríklad admin@contoso.onmicrosoft.com.
- Pred odstránením odstráňte všetky aktívne aplikácie z adresára. Ak chcete odstrániť aktívne aplikácie, prejdite na registráciu aplikácií a odstráňte existujúce aplikácie.
- V adresári nie sú priradené žiadne aktívne predplatné služieb Microsoft Online Services, ako napríklad Microsoft Azure, Office 365 alebo Azure AD Premium. Preneste svoje predplatné alebo urýchlite zrušenie aktívnych predplatných prostredníctvom podpory a fakturácie pre Azure. Ďalšie informácie nájdete v článku Zrušenie Office 365 predplatného na Azure. Pokyny na priradenie alebo pridanie existujúceho predplatného k nájomníkovi nájdete v téme Priradenie alebo pridanie predplatného služby Azure k [nájomníkovi služby Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Nie sú k dispozícii žiadne licencie Aktívne. Ak chcete odstrániť licencie, pozrite [si časť Odstránenie predplatného na odstránenie licencie.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- V adresári nie sú ako globálny správca pri pokuse o odstránenie služby Azure AD k dispozícii ďalší aktívni používatelia. Odstráňte všetkých ostatných aktívnych používateľov a je tiež potrebné odstrániť všetky závislosti od vlastného názvu domény v nájomníkovi, ako sú napríklad používatelia vytvorení pomocou admin@contoso.com.

Ďalšie podrobnosti o nasledujúcich krokoch:
- Odstráňte Azure Active Directory predplatné, pozrite si časť [Odstránenie Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Odstránenie aplikácií v adresári nájdete v téme [Odstraňovanie aplikácií.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
