---
title: Problém s otváraním alebo preberaním súborov v Yammeri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148340"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problém s otváraním alebo preberaním súborov v Yammeri

Classic Yammer podporuje viaceré možnosti pre odovzdávanie súborov do správ a skupín. V závislosti od konfigurácie siete sú súbory predvolené pre ukladanie v SharePointe.

Výber súborov v novom nariekanie zatiaľ nepodporuje všetky možnosti dostupné v klasickom nariekanie. Budúca aktualizácia pridá ďalšie funkcie. Ďalšie informácie nájdete v téme [Priloženie súboru alebo obrázka k príspevku konverzácie yammera](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Súbor sa nedá otvoriť alebo prevziať**  

Súbor sa môže nahrať do yammera, ale aj prepojenie na súbor v SharePointe Online. Ak chcete riešiť problémy, najprv musíte určiť umiestnenie súboru. Ak bol súbor odovzdaný na sieť Yammer, bude mať adresu URL *.yammer.com. Skontrolujte, či sú požadované adresy URL a adresy IP odblokované. Ďalšie informácie nájdete v blogovom príspevku [Používanie pevných kódovaných adries IP pre yammer sa neodporúča](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Skontrolujte, či používateľ, ktorý je tiež globálnym správcom, môže súbor prevziať. Ak je súbor súkromný, možno budete musieť použiť režim súkromného obsahu. Ďalšie informácie nájdete v téme [Sledovanie súkromného obsahu v yammeri](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Hostia a súbory na úrovni siete Yammer v SharePointe Online**  

[Na úrovni siete na úrovni siete Nariekanie](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nepoužívajte Azure AD B2B a sú interné nariekanie služby, takže nemajú prístup k súborom yammer uložené v SharePoint. Vytvorte externéHo používateľa AAD B2B, ktorý má prístup ku knižniciam dokumentov v SharePointe Online pomocou tejto identity. Informácie o budúcej podpore hosťových hostí služby Azure AD B2B v Yammeri nájdete v téme [Podpora pre hostí spoločnosti Business-to-business (B2B) v téme Ukážka služby Yammer – podmienky pre zákazníka a najčastejšie otázky](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).