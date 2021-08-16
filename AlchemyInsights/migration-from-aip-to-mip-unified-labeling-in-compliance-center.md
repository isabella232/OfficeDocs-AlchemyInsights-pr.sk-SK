---
title: Migrácia z AIP na označenie MIP alebo zjednotené označenie v Centre dodržiavania súladu
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
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000371"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrácia z AIP na označenie MIP alebo zjednotené označenie v Centre dodržiavania súladu

Ak chcete migrovať z označení AIP do zjednoteného označenia v centre zabezpečenia a dodržiavania súladu, vykonajte nasledovné:

**Aktivácia zabezpečenia z portálu Azure**

1. Ak ste tak ešte neurobili, otvorte nové okno prehliadača a [prihláste sa na portál Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Prejdite na **blade Azure Information Protection.** Napríklad v ponuke Centrum kliknite na položku **Všetky služby** a do poľa Filter **začnite** zadávať informácie. Vyberte **položku Azure Information Protection**. Ak ste doteraz nemali prístup k aplikácii Azure Information [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Protection, pozrite si jednočasové ďalšie kroky na pridanie tohto blade na portál. Ak chcete otvoriť aplikáciu Azure Information Protection blade, musíte mať plán [Azure Information Protection Premium alebo](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) plán Office 365, ktorý obsahuje správu prístupových práv. Ak máte niektoré z týchto predplatných, ale zobrazuje sa hlásenie, že platné predplatné nie je možné nájsť, obráťte sa na technickú podporu spoločnosti [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) alebo použite štandardné kanály podpory.

2. Vyhľadajte možnosti **ponuky Spravovať** a vyberte položku **Aktivácia zabezpečenia**. Kliknite **na položku** Aktivovať a potom potvrďte akciu. Po dokončení aktivácie sa na informačnom paneli zobrazí hlásenie **Aktivácia sa úspešne dokončila.**

**Migrácia označení Azure Information Protection do centra Office 365 zabezpečenia & súladu**

1. Prihláste sa ako používateľ s povolením globálneho správcu.

2. Prejdite na **blade Azure Information Protection.**

3. V ponuke **Spravovať** vyberte položku **Zjednotené označovanie**.

4. Na obrazovke **Azure Information Protection – Unified labeling** blade kliknite na položku **Aktivovať a** postupujte podľa online pokynov.

**Poznámka:** Pred aktiváciou migrácie Centra zabezpečenia a dodržiavania súladu overte, či & príslušné povolenia. Ďalšie informácie nájdete v týchto článkoch:

1. [Potrebujete byť globálnym správcom na konfiguráciu služby Azure Information Protection alebo môžem delegovať na iných správcov?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Dôležité informácie o rolách správcu po migrácii do centra zabezpečenia & súladu.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Ďalšie informácie o AIP do zjednotenej migrácie označení do Centra zabezpečenia a dodržiavania súladu nájdete v téme [Migrácia označení.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
