---
title: Politiky týkajúce sa hesiel
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040845"
---
# <a name="password-policies"></a>Politiky týkajúce sa hesiel

**Mám problémy s politikou hesiel pre používateľa**

- Politika hesiel používateľa závisí od toho, či je používateľ len cloud alebo lokálny.
- Cloudové len používatelia si musia vybrať heslo, ktoré spĺňa požiadavky uvedené v tomto článku: Politiky hesiel, ktoré sa vzťahujú len [na používateľské kontá cloudu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Lokálni používatelia musia vybrať heslo, ktoré spĺňa lokálne požiadavky. Ak lokálny používateľ nedokáže nastaviť svoje heslo, skontrolujte svoje lokálne požiadavky.

**Neviem, ako nastaviť alebo skontrolovať politiky uplynutia platnosti hesla**

- Pomocou prostredia PowerShell môžete nastaviť a skontrolovať politiku uplynutia platnosti pre používateľov cloudu v nájomníkovi. Postupujte podľa pokynov v tomto článku: [Nastavenie alebo kontrola politík hesiel pomocou prostredia PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Politika uplynutia platnosti hesla pre lokálnych používateľov je nastavená v lokálnej službe AD.

**Ďalšie užitočné prepojenia:**
- [Začíname s obnovením hesla](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Riešenie problémov s obnovením hesiel zo strany správcu](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
