---
title: Migrácia z AIP na MDC/zjednotené označenie v centre dodržiavania súladu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674341"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrácia z AIP na MDC/zjednotené označenie v centre dodržiavania súladu

Ak chcete migrovať z menoviek AIP na zjednotené označenie v centre zabezpečenia a dodržiavania súladu, postupujte takto:

**Aktivácia ochrany na portáli Azure**

1. Ak ste to ešte neurobili, Otvorte nové okno prehliadača a [Prihláste sa na portáli Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Prejdite na čepeľ na **ochranu informácií v Azure** . V ponuke rozbočovač kliknite napríklad na položku **všetky služby** a začnite písať **informácie** do poľa Filter. Vyberte položku **Azure Information Protection**. Ak ste sa ešte nedostali do programu Azure Information Protection Blade, pozrite si jednorazové [Ďalšie kroky](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) na pridanie tohto kotúča na portál. Ak chcete otvoriť čepeľ na ochranu informácií o Azure, musíte mať [plán služieb Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) alebo plán služieb Office 365, ktorý obsahuje správu prístupových práv. Ak máte niektorý z týchto predplatných, ale zobrazí sa hlásenie o tom, že platné predplatné sa nenašlo, obráťte sa na oddelenie technickej podpory [spoločnosti Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) alebo použite štandardné podporné kanály.

2. Vyhľadajte možnosti ponuky **Spravovať** a vyberte položku **Aktivácia ochrany**. Kliknite na položku **aktivovať**a potvrďte akciu. Po dokončení aktivácie sa na informačnom paneli zobrazí hlásenie **Aktivácia sa úspešne dokončila**.

**Migrácia menoviek Azure Information Protection na centrum zabezpečenia & zabezpečenia dodržiavania súladu v Office 365**

1. Skontrolujte, či ste prihlásení ako používateľ s povolením globálneho správcu.

2. Prejdite na čepeľ na **ochranu informácií v Azure** .

3. V ponuke **Spravovať** vyberte možnosť **Unified labeling (zjednotené označenie**).

4. Na karte **Azure Information Protection – Unified labeling** Blade kliknite na položku **aktivovať** a postupujte podľa pokynov online.

**Poznámka**: Skontrolujte, či máte príslušné povolenia pred aktiváciou migrácie centra zabezpečenia & súladu. Ďalšie informácie nájdete v týchto článkoch:

1. [Musíte byť globálnym správcom na konfiguráciu služby Azure Information Protection alebo môžem delegovať na iných správcov?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Dôležité informácie o rolách správcu po migrácii do centra zabezpečenia & dodržiavania súladu.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Ďalšie informácie o AIP na zjednotené označenie migrácie do centra zabezpečenia a dodržiavania súladu nájdete v téme [migrácia menoviek](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
