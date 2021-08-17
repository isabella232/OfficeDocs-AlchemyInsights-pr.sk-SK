---
title: Oprava politiky nájomníka (prepísanie akcie)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896090"
---
# <a name="fix-tenant-policy-action-override"></a>Oprava politiky nájomníka (prepísanie akcie)

Toto hlásenie ovplyvnila jedna z vašich politík ochrany pred nevyžiadanou poštou. Ak chcete skontrolovať politiky, postupujte takto:

1. Na portáli Microsoft 365 Defender prejdite na položku Politiky spolupráce pre <https://security.microsoft.com/>  \>  \>  \> **e-&**  na & Pravidlá politiky hrozieb Ochrana pred nevyžiadanou poštou v časti Politiky.

   Ak chcete prejsť priamo na stránku **Politiky ochrany pred nevyžiadanou poštou,** <https://security.microsoft.com/antispam> použite .

2. Na stránke Politiky **ochrany** pred nevyžiadanou poštou vyberte politiku kliknutím na  názov politiky **(**  Typ je Vlastná politika ochrany pred nevyžiadanou poštou alebo Názov je politika prichádzajúcej pošty proti nevyžiadanej pošte **(predvolená možnosť)).**
3. V zobrazenej bubline s podrobnosťami vyberte položku **Upraviť akcie** v **časti** Akcie.
4. Ak chcete **zistiť,** či sú vybraté niektoré z týchto hodnôt,  v časti Akcie so správami si prečítajte verdikt nevyžiadanej **pošty,** nevyžiadanú poštu s vysokou spoľahlivosťou, neoprávnené získavanie údajov s vysokou spoľahlivosťou:
   - **Pridanie hlavičky X**
   - **Na predotvorenie riadku predmetu s textom**
   - **Presmerovať správu na e-mailovú adresu**
   - **Odstrániť správu**
   - **Žiadna akcia**

   Je možné, že štandardné nastavenia **sa použijú na** všetkých zákazníkov Exchange Online Protection správu ovplyvnili.

Ďalšie informácie nájdete v téme [Konfigurácia politík ochrany pred nevyžiadanou poštou v systéme EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
