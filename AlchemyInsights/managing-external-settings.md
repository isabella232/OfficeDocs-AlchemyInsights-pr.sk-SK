---
title: Správa externých nastavení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294435"
---
# <a name="managing-external-settings"></a>Správa externých nastavení

**Oznámenie**

- [Odmietanie podpory pri prihlasovaní na webové stránky od spoločnosti Google od 4. januára 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support). Otestujte, či sú vaše aplikácie ovplyvnené podľa pokynov spoločnosti Google v oblasti testovania kompatibility
- Uistite sa, že pri prihlasovaní používateľov pomocou používateľských kont Google používate systémové webové zobrazenie alebo systémový prehliadač

**Spravovanie nastavení pozvánok**

Potvrďte, že ste [nakonfigurovali nastavenie externej spolupráce](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) , aby sa umožnilo príslušným ľuďom odosielať pozvánky.

**Správa povolení na prístup používateľov hosťa**

1. Globálny správcovia môžu spravovať povolenia hosťovského prístupu v adresári prostredníctvom portálu Azure konfiguráciou povolení na prístup hostí na stránke externého nastavenia spolupráce. Ďalšie [informácie o tomto nastavení](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).
2. Ak chcete, aby mali hostia prístup k aplikáciám, ako sú napríklad aplikácie teams alebo SharePoint, potvrďte, že ste nakonfigurovali tieto aplikácie, aby umožnili prístup hostí. Ďalšie informácie o [nastaveniach tímov](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) a [SharePointe](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).

**Konfigurovanie pozvánok:**

- [Povolenie externej spolupráce B2B a spravovanie osôb, ktoré môžu pozvať hostí](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Povolenie alebo blokovanie pozvánok používateľom z konkrétnych organizácií](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurovanie povolených poskytovateľov identity:**

- [Federácia služby Google](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Priama federácia](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Overenie e-mailu jedným časovým heslom](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
