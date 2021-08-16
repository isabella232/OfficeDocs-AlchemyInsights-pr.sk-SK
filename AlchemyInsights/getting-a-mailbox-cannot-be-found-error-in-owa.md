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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056505"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Zobrazuje sa vám chyba o tom, že sa poštová Outlook na webe?

Ak používate Outlook na webe **a** zobrazí sa chybové hlásenie o poštovej schránke, konto, ktoré ste použili na pripojenie k službe Outlook na webe, nemá licenciu na Exchange Online, a preto ku kontu nie je priradená žiadna poštová schránka. Správca môže vášmu kontu priradiť licenciu pomocou týchto krokov:

1. Otvorte dialógové [Centrum spravovania služby Microsoft 365](https://portal.office.com/adminportal/home#/homepage) prejdite na položku **Aktívni** používatelia v časti Používatelia a vyberte používateľa, ktorý chybu zobrazuje. 

2. Na stránke používateľa, ktorá sa  otvorí, prejdite do časti  Licencie a aplikácie, vyberte príslušnú hodnotu Umiestnenia a priraďte licenciu, ktorá obsahuje Exchange Online (rozbaľte licenciu a zobrazte jej podrobnosti). Po dokončení kliknite na tlačidlo **Uložiť zmeny**.

V niektorých prípadoch, ak je licencia už priradená k používateľskému kontu, odstránenie a opätovné priradenie licencie pomáha vyriešiť problém a správne ho poskytnúť v systéme: 

- Skontrolujte, či sú vaše predplatné služby M365 Exchange Online (a iné, ak nejaké máte) aktuálne a či nemáte nedávno uplynutú platnosť.

Keď ste sa uistili, že platnosť predplatného nelynula a ku kontu používateľa bola priradená platná licencia, môže trvať až 24 hodín, kým sa zistí platnosť licencie, takže možno budete musieť počkať, kým sa problém vyrieši. Ďalšie informácie nájdete v téme [Priradenie a správa licencií.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)