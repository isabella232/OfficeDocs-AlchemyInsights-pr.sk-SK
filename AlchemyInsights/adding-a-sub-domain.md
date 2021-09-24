---
title: Pridanie subdoméie
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506771"
---
# <a name="adding-a-sub-domain"></a>Pridanie subdoméie

Subdomémy je možné pridať k rovnakému alebo odlišnému nájomníkovi ako nadradená doména. V oboch prípadoch musíte spravovať svoje vlastné nastavenia na webovej lokalite registrátora. Ak ste chceli spoločnosti Microsoft spravovať nastavenia DNS pomocou NS záznamov alebo ste doménu kúpili od spoločnosti Microsoft, subdomény nie je možné pridávať bez toho, aby ste toto predchádzajúceho nastavenia menili.

Najskôr pridajte nadradenú doménu a potom pridajte vedľajšiu doménu. Ak sa subdoména nachádza v tom istom nájomníkovi, nie je potrebné žiadne ďalšie overenie. Ak pridáte subdoméu k samostatnému nájomníkovi, na overenie vlastníctva sa vyžaduje txt záznam DNS ešte pred pridaním domény a ďalších DNS záznamov pre vybraté služby.

- Ak chcete pridať doménu alebo [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)subdoménu, postupujte podľa sprievodcu pridaním domény alebo manuálne pridajte doménu alebo subdoménu tak, že otvoríte nastavenie  >  **domény**  >  **Pridať doménu.**

V prípade potreby:

- Ak chcete zmeniť správcu nastavení DNS pre existujúcu doménu, prejdite do časti **Nastavenia** Domains (Domény) , začiarknite políčko vedľa domény a  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)potom vyberte položku Manage **DNS (Spravovať DNS).** V sprievodcovi vyberte položku **Pridať vlastné DNS záznamy a** dokončite sprievodcu.
- Ak chcete pridať subdoménu do domény zakúpenej spoločnosťou Microsoft, najprv preneste doménu k inému registrátorovi a potom vykonajte vyššie uvedenú zmenu na spravovanie vlastných DNS záznamov. Pokyny nájdete v téme [Prenos domény od spoločnosti Microsoft k inému hostiteľovi](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Ak sa zobrazí chyba, že vašu doménu už používajú iní členovia alebo ľudia vo vašej organizácii, musíte pred použitím domény prevziať toto nespravované konto. Pokyny nájdete v [téme Prevziať nespravovaný adresár ako správca v Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)
