---
title: Riešenie problémov s kódmi chýb služby Azure AD Authentication and Authorization (AADSTS)
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
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037838"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Riešenie problémov s kódmi chýb služby Azure AD Authentication and Authorization (AADSTS)

Ak chcete vyriešiť kódy chýb overenia a autorizácie AAD (AADSTS), vykonajte tieto Odporúčané kroky:

1. **Manipulácia s kódmi chýb v aplikácii**

- **OAuth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 poskytuje usmernenie o tom, ako zvládnuť chyby počas overovania s použitím chybovej časti odpovede na chybu.

    - **chyba**: reťazec kódu chyby, ktorý sa môže použiť na klasifikáciu typov chýb, ktoré sa vyskytujú, a mali by sa použiť na reakciu na chyby.
    - Pole **chyby** obsahuje niekoľko možných hodnôt – Preskúmajte prepojenia na dokumentáciu k protokolom a špecifikácie OAuth 2,0 a získajte ďalšie informácie o konkrétnych chybách a o tom, ako na ne reagovať.

- Tu je ukážka odpovede na chyby:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Informácie o aktuálnom kóde chyby vyhľadávania**

- Kódy chýb a správy sa môžu zmeniť. Najaktuálnejšie informácie nájdete v téme https://login.microsoftonline.com/error Vyhľadanie AADSTS chýb, opráv a niektorých navrhovaných alternatívnych riešení.
- Môžete tiež vyhľadať a riešiť problémy s [kódmi chýb AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) uvedených v článku [Azure AD Authentication and Authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Získanie pomoci**

- [Možnosti podpory a Pomocníka pre vývojárov](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – Ak potrebujete odpoveď na otázku alebo pomoc pri riešení problému, ktorý nie je obsiahnutý v našej dokumentácii, môže sa stať, že budete môcť získať pomoc odborníkom. Tento článok obsahuje niekoľko návrhov na získanie odpovedí na otázky počas vývoja aplikácií, ktoré sú integrované s platformou Microsoft Identity.








