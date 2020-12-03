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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564881"
---
# <a name="delete-tenant"></a>Odstrániť nájomníka

Ak chcete odstrániť Azure AD, zabezpečte:
- Ste globálnym správcom v adresári.
- NIE ste prihlásení s kontom, ktoré má predvolený adresár, napríklad contoso.onmicrosoft.com, v prihlasovacom konte, ako je napríklad admin@contoso.onmicrosoft.com.
- Pred odstránením odstráňte všetky aktívne aplikácie v adresári. Ak chcete odstrániť aktívne aplikácie, prejdite na položku registrácie aplikácií a odstráňte existujúce aplikácie.
- Neexistujú žiadne aktívne predplatné na žiadne služby Microsoft Online Services, ako je napríklad Microsoft Azure, Office 365 alebo Azure AD Premium, ktoré sú priradené k adresáru. Prenášajte predplatné alebo Zrýchlite zrušenie aktívnych predplatných prostredníctvom podpory Azure a fakturácie. Ďalšie informácie o zrušení predplatného na Office 365 a Azure. Pokyny na priradenie alebo Pridanie existujúceho predplatného nájomníkovi nájdete v téme [Priradenie alebo pridanie predplatného Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- K dispozícii nie sú žiadne aktívne licencie. Ak chcete odstrániť licencie, pozrite si tému [Odstránenie predplatného na odstránenie licencie](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Pri pokuse o odstránenie Azure AD sa nenachádzajú žiadne ďalšie aktívni používatelia v adresári okrem seba ako globálny správca. Odstráňte všetkých ostatných aktívnych používateľov a všetky závislosti na vlastnom názve domény v nájomníkovi budú tiež potrebné odstrániť, ako napríklad používatelia vytvorené pomocou admin@contoso.com.

Ďalšie podrobnosti nájdete v téme postup:
- Odstránenie služby Azure Active Directory alebo predplatného nájdete v téme [Odstránenie Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Odstraňujú sa aplikácie v adresári, pozrite si tému [odstránenie aplikácií](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
