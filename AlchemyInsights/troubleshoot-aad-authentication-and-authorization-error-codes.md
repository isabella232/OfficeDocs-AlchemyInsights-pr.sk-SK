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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="c943b-102">Riešenie problémov s kódmi chýb služby Azure AD Authentication and Authorization (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="c943b-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="c943b-103">Ak chcete vyriešiť kódy chýb overenia a autorizácie AAD (AADSTS), vykonajte tieto Odporúčané kroky:</span><span class="sxs-lookup"><span data-stu-id="c943b-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="c943b-104">**Manipulácia s kódmi chýb v aplikácii**</span><span class="sxs-lookup"><span data-stu-id="c943b-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="c943b-105">**OAuth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 poskytuje usmernenie o tom, ako zvládnuť chyby počas overovania s použitím chybovej časti odpovede na chybu.</span><span class="sxs-lookup"><span data-stu-id="c943b-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="c943b-106">**chyba**: reťazec kódu chyby, ktorý sa môže použiť na klasifikáciu typov chýb, ktoré sa vyskytujú, a mali by sa použiť na reakciu na chyby.</span><span class="sxs-lookup"><span data-stu-id="c943b-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="c943b-107">Pole **chyby** obsahuje niekoľko možných hodnôt – Preskúmajte prepojenia na dokumentáciu k protokolom a špecifikácie OAuth 2,0 a získajte ďalšie informácie o konkrétnych chybách a o tom, ako na ne reagovať.</span><span class="sxs-lookup"><span data-stu-id="c943b-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="c943b-108">Tu je ukážka odpovede na chyby:</span><span class="sxs-lookup"><span data-stu-id="c943b-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="c943b-109">**Informácie o aktuálnom kóde chyby vyhľadávania**</span><span class="sxs-lookup"><span data-stu-id="c943b-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="c943b-110">Kódy chýb a správy sa môžu zmeniť.</span><span class="sxs-lookup"><span data-stu-id="c943b-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="c943b-111">Najaktuálnejšie informácie nájdete v téme https://login.microsoftonline.com/error Vyhľadanie AADSTS chýb, opráv a niektorých navrhovaných alternatívnych riešení.</span><span class="sxs-lookup"><span data-stu-id="c943b-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="c943b-112">Môžete tiež vyhľadať a riešiť problémy s [kódmi chýb AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) uvedených v článku [Azure AD Authentication and Authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="c943b-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="c943b-113">**Získanie pomoci**</span><span class="sxs-lookup"><span data-stu-id="c943b-113">**Get Help**</span></span>

- <span data-ttu-id="c943b-114">[Možnosti podpory a Pomocníka pre vývojárov](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – Ak potrebujete odpoveď na otázku alebo pomoc pri riešení problému, ktorý nie je obsiahnutý v našej dokumentácii, môže sa stať, že budete môcť získať pomoc odborníkom.</span><span class="sxs-lookup"><span data-stu-id="c943b-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="c943b-115">Tento článok obsahuje niekoľko návrhov na získanie odpovedí na otázky počas vývoja aplikácií, ktoré sú integrované s platformou Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="c943b-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








