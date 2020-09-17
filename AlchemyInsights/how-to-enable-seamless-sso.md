---
title: Povolenie bezproblémového SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780542"
---
# <a name="how-to-enable-seamless-sso"></a>Povolenie bezproblémového SSO

Povoliť bezproblémové SSO prostredníctvom služby [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Ak vytvárate novú inštaláciu služby Azure AD Connect, vyberte [vlastnú cestu inštalácie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). Na **prihlasovacej stránke používateľa** vyberte možnosť **Povoliť jediné prihlásenie** .
  
Ak chcete overiť, či ste správne povolili bezproblémové prihlásenie:
  
1. Prihláste sa do [centra spravovania služby Azure Active Directory](https://aad.portal.azure.com) ako globálny správca.

2. Na ľavej table vyberte položku **Azure Active Directory** .

3. Overte, či je **zapnuté**bezproblémové jediné prihlásenie.

Ďalšie informácie nájdete v téme [jednoduché prihlásenie v službe Azure Active Directory: rýchly začiatok](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  