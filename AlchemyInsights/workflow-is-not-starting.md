---
title: Tok činností sa nespustí
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270795"
---
# <a name="workflow-is-not-starting"></a>Tok činností sa nespustí

- Pracovné postupy služby SharePoint 2010 a SharePoint 2013 sa nespustí.

    - Ak váš pracovný postup sa nedá spustiť, tam môže byť problém pri dočasnej služby tam, kde používatelia môžu vyskytnúť občasné meškanie s workflow pokrok. Kontrola [Tabuľa stav služby](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) zistiť, ak vaša organizácia je ovplyvnené.

    - Ak uplynulo viac ako 24 hodín od najprv ste videli tento problém, prihláste sa prosím na podporu lístok. V mnohých prípadoch už pracujeme na riešení. Prosím, dajte nám aspoň 24 hodín na kompletné riešenie.

- Pracovné postupy služby SharePoint 2010 odložené na Štart.

    - V takom prípade pracovný postup sa spustí vo veľkých sériách. (napríklad keď niekoľko položky sú pridané naraz).

    - Toky činností nie sú určené na spustiť v reálnom čase, takže oneskorenie je-design správanie.

   -  Ak tok činností je zložité Extensible Object Markup jazyk (XMol) od, kompilácia môže byť pomalé. Pozrite [Tento](https://support.microsoft.com/en-us/kb/3043697) článok.

    - By mala zjednodušiť pracovného postupu alebo redesign pomocou typ platformy Microsoft SharePoint 2013 pracovného postupu.

    - Ak históriu toku činností Veľká, chcete položky vymazať alebo vytvoriť nový zoznam histórie.

        Viac informácií: [Vymazanie histórie toku činností](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Súvisiace témy
Chceš skúsiť Flow Microsoft SharePoint Online?
- [Vytvoriť tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


