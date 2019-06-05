---
title: Vytvorenie a používanie zdieľanej poštovej schránky
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717361"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Vyriešiť problém - používateľ nenašiel v adresári

<p>Používateľom sa zobrazuje chybové hlásenie <strong> &ldquo; &hellip;používateľ môže&rsquo;t nájsť v adresári. Prosím skúste to znova&hellip; </strong> kde je problém typ <strong> &ldquo;nie je v adresári.&rdquo;</strong>, tieto kroky môže byť dokončená na vyriešenie problému.</p> <ol> <li>Zabezpečiť konto, e-mailovú pozvánku prijme rovnaké konto, ktoré používa prihlásiť neskôr. Uistite sa, že používateľ používa rovnaké konto prijmite pozvanie a prihláste sa do site. <br /><br />Pre viac informácií, pozrite si <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">Správa aliasov konta Microsoft</a> spravovať Office 365 prihlásenie. <br /><br /></li> <li>Vyhľadajte každý lokalít, v ktorých používateľ dostáva chyba. <br /><br />a. Pridať <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (do úvodzoviek) na koniec URL stránky. <br /><br />Príklad: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Vyberte používateľa v zozname. <br /><br />c. Kliknite na položku <strong>odstrániť povolenia používateľov z pásky</strong>. <br /><br />d. Pridať späť používateľa a odoslať pozvánku používateľovi.</li> </ol>

