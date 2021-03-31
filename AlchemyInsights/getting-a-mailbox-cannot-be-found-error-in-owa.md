---
title: 126 Nepodarilo sa v aplikácii OWA nájsť chybu o získaní poštovej schránky?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426677"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Zobrazuje sa vám v Outlooku na webe chyba o tom, že sa poštová schránka nenašiel?

Ak používate Outlook na webe **a** poštovú schránku sa nepodarilo nájsť z dôvodu chyby, konto, ktoré ste použili na pripojenie k Outlooku na webe, nemá licenciu na Exchange Online, a preto ku kontu nie je priradená žiadna poštová schránka. Správca môže vášmu kontu priradiť licenciu pomocou týchto krokov:

1. Otvorte Centrum [spravovania služby Microsoft 365,](https://portal.office.com/adminportal/home#/homepage) prejdite do časti Aktívni používatelia v časti Používatelia a vyberte používateľa, ktorý chybu zobrazuje.  

2. Na stránke používateľa, ktorá sa  otvorí, prejdite do časti  Licencie a aplikácie, vyberte príslušnú hodnotu Umiestnenia a priraďte licenciu, ktorá obsahuje Exchange Online (rozbaľte licenciu a zobrazte jej podrobnosti). Po dokončení kliknite na tlačidlo **Uložiť zmeny**.

V niektorých prípadoch, ak je licencia už priradená k používateľskému kontu, odstránenie a opätovné priradenie licencie pomáha vyriešiť problém a správne ho poskytnúť v systéme: 

- Skontrolujte, či sú vaše predplatné na M365 Exchange Online (a iné, ak máte nejaké) aktuálne a či uplynula platnosť len nedávno.

Keď ste sa uistili, že platnosť predplatného nelynula a ku kontu používateľa bola priradená platná licencia, môže trvať až 24 hodín, kým sa zistí platnosť licencie, takže možno budete musieť počkať, kým sa problém vyrieši. Ďalšie informácie nájdete v téme [Priradenie a správa licencií.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)