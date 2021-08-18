---
title: Konfigurovanie LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090427"
---
# <a name="configure-ldap"></a>Konfigurovanie LDAP

Ak chcete nakonfigurovať LDAP, vykonajte nasledovné kroky:

1. Skontrolujte stav svojej domény na [portáli Azure.](https://aka.ms/aadds-health)
1. Skontrolujte, či je k dispozícii platné predplatné na Azure AD a či sú povolené doménové služby Azure AD.
1. Certifikát vyžadovaný na povolenie zabezpečeného protokolu LDAP musí byť získaný od dôveryhodnej verejnej certifikačnej autority alebo musí byť certifikátom s vlastným podpisom.
1. Uistite sa, že certifikát dodržiava požadované [pokyny.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Neplatný certifikát**
1. Ak chcete obnoviť certifikát, postupujte podľa krokov na vytvorenie nového certifikátu a opätovné zaťaženie: [Nakonfigurujte LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Ak chcete vyriešiť známy problém s upozorneniami secure LDAP v doménových službách Azure Active Directory, pozrite si [tému Riešenie upozornení LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
