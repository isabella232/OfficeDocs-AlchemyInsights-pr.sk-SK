---
title: Pracovný postup sa nes začatím
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907753"
---
# <a name="workflow-is-not-starting"></a>Pracovný postup sa nes začatím

- SharePoint 2010 a SharePoint 2013 sa nesajú.

    - Ak sa pracovný postup nes začatím nezačína, môže ísť o dočasný problém so službami, v rámci ktorého sa používateľom môžu vyskytnúť občasné oneskorenia s priebehom pracovného postupu. Skontrolujte [tabuľu stavu služby a](https://admin.microsoft.com/AdminPortal/Home/servicehealth) zistite, či to bude mať vplyv na vašu organizáciu.

    - Ak uplynulo viac než 24 hodín od toho, čo ste tento problém prvýkrát videli, prihláste sa do lístka technickej podpory. V mnohých prípadoch už pracujeme na riešení. Dajte nám aspoň 24 hodín na dokončenie riešenia.

- SharePoint spustení sa odložili pracovné postupy z roku 2010.

    - Dochádza k tomu, ak sa pracovný postup spustí vo veľkých dávkach. (napríklad, keď sa pridá niekoľko položiek naraz).

    - Pracovné postupy nie sú navrhnuté na spustenie v reálnom čase, preto je oneskorenie v štýle návrhu.

   -  Ak je pracovný postup komplexný extensible Object Markup Language (XILE), kompilácia môže byť pomalá. Pozrite [si tento](https://support.microsoft.com//kb/3043697) článok.

    - Pracovný postup by ste mali zjednodušiť alebo ho vylepšiť pomocou typu platformy Microsoft SharePoint 2013 Workflow.

    - Ak sa história pracovného postupu príliš rozrástla, môžete položky vymazať alebo vytvoriť nový zoznam histórie.

        Ďalšie informácie: [Vymazanie histórie pracovného postupu](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Súvisiace témy
Chcete sa o Microsoft Flow v SharePoint Online?
- [Vytvorenie Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
