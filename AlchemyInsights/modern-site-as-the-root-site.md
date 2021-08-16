---
title: Moderná lokalita ako koreňová lokalita
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000407"
---
# <a name="modern-site-as-root-site"></a>Moderná lokalita ako koreňová lokalita

Začali sme s zavádzanie novej funkcie, ktorá vám umožní vymeniť klasickú koreňovú lokalitu [lokality s modernou stránkou.](https://docs.microsoft.com/sharepoint/modern-root-site) Ak chcete pri archivácii pôvodnej lokality vymeniť umiestnenie lokality s inou stránkou, použite možnosť [Invoke-SPOSiteSwap.](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) K dispozícii pre tímovú lokalitu (nie je pripojená ku skupine) aj pre komunikačnú lokalitu.

>[!Important]
> Ak chcete vytvoriť modernú komunikačnú lokalitu, neodstránijte klasickú koreňovú lokalitu. Spoločnosť Microsoft túto aplikáciu nepodporuje. Odstránením koreňovej lokality budú všetky lokality SharePoint vo vašej organizácii neprístupné pre všetkých používateľov, kým lokalitu obnoviť alebo vytvoriť novú lokalitu s rovnakou URL adresou. Túto funkciu budeme o tejto funkcii komunikovať prostredníctvom centra správ. Očakávate, že funkcia bude v nájomníkovi zakrátko zapnutá.

## <a name="known-issues-with-swapping-sites"></a>Známe problémy s výmenou lokalít
- Cieľová lokalita môže na krátky čas vrátiť chybu "nenašiel sa" (HTTP 404).
- Ak chcete aktualizovať index vyhľadávania, obsah sa bude musieť opätovne uchýliť. V tomto prípade nie je potrebný žiadny manuálny krok, táto postup sa vykonáva automaticky.
- Všetko závislé od "statických" prepojení (napríklad synchronizácia súborov a odstránenie OneNote súborov) bude potrebné manuálne opraviť.
- Project Na to, aby sa aj naďalej pridruželi správne, možno bude potrebné overiť lokality servera. 
