---
title: Synchronizácia hash hesla pre službu Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177622"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Synchronizácia hash hesla pre službu Domain

**Ak sa na inštanciu služby Azure AD DS zobrazí výzva na povolenie synchronizácie hash hesla**

Narazíte na scenár, v ktorom používate hybridné prostredie s používateľmi, ktorí synchronizujú z lokálneho prostredia služby Azure Active Directory Domain Services (AD DS). Tento scenár sa vyskytuje napriek tomu, že sa Synchronizácia hash hesla z lokálneho AD DS na nájomníka služby Azure AD nachádza.

**Príčina**

To sa deje, pretože Azure AD Connect predvolene nesynchronizuje staršie nové technológie LAN Manager (NTLM) a Kerberos Password hash, ktoré sú potrebné pre Azure AD DS.

**Alternatívne riešenie** 

Ak chcete synchronizovať tieto hodnoty hash hesla vyžadované pre overovanie NTLM a Kerberos, budete musieť nakonfigurovať službu Azure AD Connect.

Po nakonfigurovaní služby Azure AD Connect sa pri vytvorení lokálneho konta alebo udalosti zmeny hesla potom synchronizuje staršie hash hesla k službe Azure AD. Ďalšie informácie o tejto téme a pokyny na Zapnutie synchronizácie hesiel v hybridných prostrediach Azure AD DS nájdete [tu](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) .