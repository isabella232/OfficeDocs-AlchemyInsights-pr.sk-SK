---
title: Workflow e-mail sa odosiela nie
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270687"
---
# <a name="workflow-email-is-not-being-sent"></a>Workflow e-mail sa odosiela nie

1. E-mail od toky činností nie sú odoslané do všetkých používateľov alebo iba určitým používateľom alebo vidíte chybu **e-mailovú správu nemožno odoslať. Uistite sa, e-mailu má platný príjemcu**.

    Skontrolujte, či používateľ existovať v skupine povolenia **Všetkým ľuďom** (zoznam informácií o používateľoch) pre túto kolekciu lokalít.  Ochutnajte priame URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Ak používateľ neexistuje, uistite sa, že používateľ je podpísaná do stránky. 
    - Ak je externého používateľa, uistite sa, že ich pozvania.
    - Ak používateľ neexistuje v skupine povolenia, uistite sa, že e-mailová adresa je správna.
    - Ak užívatelia e-mailová adresa je tu, potom vytvoriť ukážku upozornenia pre daného používateľa, ktorá núti synchronizácie používateľského konta z používateľské profily SharePoint do kolekcie lokality.
 
2. E-mail od pracovných postupov sa odosielajú správcovia kolekcie lokalít, ale nie iných používateľov a zobraziť chyba **HTTP zakázané na <spam> <spam> ** <spam> <spam>.
 

    Vidieť [Prístup odmietnutý pri e-mail do skupiny](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Tiež skontrolujte, že funkcie kolekcie lokality **obmedzeným prístupom používateľ povolenie uzamknutie režime** nie je aktívny.


## <a name="related-topics"></a>Súvisiace témy
Chceš skúsiť Flow Microsoft SharePoint Online?
- [Vytvoriť tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


