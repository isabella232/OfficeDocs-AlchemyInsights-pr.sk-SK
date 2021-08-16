---
title: Oznámenia v Yammeri
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097213"
---
# <a name="notifications-in-yammer"></a>Oznámenia v Yammeri

[Yammer odosiela oznámenia](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) na upozorňovanie na novú aktivitu v príslušných konverzáciách e-mailom alebo, ak používate Yammer v mobilnom zariadení, prostredníctvom push oznámení. Yammer predvolene odosiela oznámenia pre mnohé typy aktivít vo vašej sieti. Používatelia môžu aktualizovať svoje nastavenia e-mailu prostredníctvom webovej lokality Yammera a push oznámenia sa konfigurujú prostredníctvom mobilnej aplikácie. 

Yammer už podporuje aj [interaktívne e-maily v Outlooku](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Niektoré e-maily (kópie správ) sa v Outlooku na webe stanú interaktívnymi. V niektorej z budúcich aktualizácií sa táto funkcia dostane aj do ďalších verzií Outlooku.

**Typy oznámení v Yammeri**

- E-maily (Aktualizácie zo skupiny, niekto vás pozve do skupiny, dostanete správu do priečinka doručenej pošty atď.)
- Push oznámenia (Odosielané do mobilných zariadení, keď vás niekto zmieni, keď dostanete správu do priečinka doručenej pošty atď.)
- Oznámenia na pracovnej ploche (Ak máte nainštalovanú počítačovú aplikáciu Yammer, zobrazujú sa kontextové oznámenia.)
- Oznámenia s ikonou zvončeka (Na webovej lokalite Yammera sa používateľom zobrazujú oznámenia o rôznych udalostiach. Tieto oznámenia nemusia vždy mať súvisiace e-mailové alebo push oznámenie.)

Pozrite si [podrobnejšie informácie o oznámeniach](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Spravovanie oznámení**

Používatelia si oznámenia spravujú sami. Pozrite si informácie o tom, [ako zapnúť a vypnúť e-mailové a mobilné oznámenia Yammera](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Nie je možné, aby správcovia zakázali všetky oznámenia ani ovládali oznámenia v mene používateľov. Správcovia môžu [ovládať logo zahrnuté do e-mailov a tiež to, či používatelia musia potvrdiť správy](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) odoslané e-mailom.

**E-mailové oznámenia odoslané mnohým používateľom vo vašej organizácii**

Niekedy sa stane, že jedno e-mailové oznámenie odoslané Yammerom dostane viac používateľov v organizácii, ako sa očakávalo. Stáva sa to vtedy, keď sa do Yammera pridá distribučný zoznam alebo iný typ inej ako individuálnej e-mailovej adresy. Yammer niekedy nevie, či e-mailová adresa patrí jednotlivému používateľovi alebo či ide o e-mailovú adresu, ktorá spôsobí doručenie jedného e-mailu mnohým príjemcom. Ak sa vyskytne tento problém, je potrebné vykonať opatrenie na [pozastavenie (deaktivovanie) neplatného používateľa s touto e-mailovou adresou](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) v Yammeri. 

Ak chcete znížiť pravdepodobnosť výskytu tohto problému, mali by ste:

1. [Vynútiť identitu Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) pre Yammer.
2. Zablokovať externým odosielateľom odosielanie e-mailov vašej organizácii alebo obmedziť odosielateľov na schválený zoznam.

Ak sa vyskytne tento problém:

1. Identifikujte príjemcu e-mailu, ktorý by sa mal zhodovať s používateľom v Yammeri. Napríklad predajcovia@fabrikam.com je distribučný zoznam pre všetkých predajcov. Tento distribučný zoznam by bol identifikovateľný v e-mailoch z Yammera prijatých používateľmi.
2. Pomocou funkcie [deaktivovať (pozastaviť) v správcovi siete](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) pozastavte používateľa, ktorý má e-mailovú adresu predajcovia@fabrikam.com. Pozastavenie je možné zrušiť, preto je bezpečnejšie ako odstránenie. Po 90 dňoch automaticky dôjde k odstráneniu používateľa.
3. Prípadne si prezrite [export používateľov](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), aby ste identifikovali iné ako používateľské e-mailové adresy, ktoré sa majú pozastaviť.
