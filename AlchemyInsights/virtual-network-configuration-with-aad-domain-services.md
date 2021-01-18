---
title: Virtuálna konfigurácia s doménovou službou AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885649"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuálna konfigurácia s doménovou službou AAD

Virtuálna konfigurácia s doménovou službou AAD zahŕňa tieto kroky: 

1. Kontrola stavu domény na portáli Azure https://aka.ms/aadds-health
2. Kontrola NSG pravidiel, ktoré blokujú porty potrebné na synchronizáciu v službe Azure AD Domain Services na portáli https://aka.ms/aadds-networking
3. Zabezpečte, aby bola Vaša virtuálna sieť nasadená v rovnakej oblasti Azure ako doména spravovaná doménou služby Azure AD.
4. Zabezpečte, že nemáte existujúcu doménu s rovnakým názvom domény, ktorá je k dispozícii vo virtuálnej sieti.

Ďalšie informácie o návrhu v službe Azure Virtual Network na podporu doménových služieb AAD nájdete v téme [virtuálna sieť úvaha](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

