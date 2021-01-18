---
title: Konfigurácia LDAP
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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885577"
---
# <a name="configure-ldap"></a>Konfigurácia LDAP

Ak chcete nakonfigurovať LDAP, postupujte takto:

1. Skontrolujte stav svojej domény na [portáli Azure](https://aka.ms/aadds-health).
1. Skontrolujte, či je k dispozícii platné predplatné služby Azure AD a či je povolená služba Azure AD Domain Services.
1. Certifikát potrebný na povolenie zabezpečeného LDAP musí byť získaný od dôveryhodného verejného certifikačného úradu alebo je certifikát s vlastným podpisom.
1. Skontrolujte, či sa certifikát riadi požadovanými [pokynmi](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Neplatný certifikát**
1. Ak chcete obnoviť certifikát, postupujte podľa krokov na vytvorenie nového certifikátu a opätovného nahrania: [Konfigurácia LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Ak chcete vyriešiť známy problém so zabezpečenými upozorneniami LDAP v doménových službách Azure Active Directory, pozrite si tému [vyriešenie upozornení LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
