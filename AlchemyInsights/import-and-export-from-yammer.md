---
title: Importovanie a exportovanie z Yammera
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037259"
---
# <a name="import-and-export-from-yammer"></a>Importovanie a exportovanie z Yammera

**Importovať**

Možnosti importovania používateľov sa líšia v závislosti od toho, či je vaša sieť Yammer v [natívnom režime pre Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)alebo nie.

- **Nenatívny režim**: používatelia môžu byť importovaní do skupín pomocou položky [Pridať z adresára](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (obmedziť na 100 používateľov) v rámci nastavenia skupiny alebo do siete s použitím [hromadnej aktualizácie](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) v správcovi siete.
- **Natívny režim**: členstvo v skupine a operácie členstva v sieti by sa mali vykonávať na [portáli Microsoft 365 admin Portal](https://docs.microsoft.com/microsoft-365/admin/add-users), v službe [Azure AD Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)alebo pomocou inej možnosti služby Azure AD. Siete v natívnom režime už nemajú prístup k hromadnej aktualizácii a iným starším funkciám.

> [!IMPORTANT]
> Yammer nikdy nepodporoval Importovanie obsahu v správcovi siete, a to ani v prípade, že funkcia exportu údajov bola použitá v inej sieti. Obsah môže byť opätovne odoslaný partnerskými riešeniami alebo rozhraniami Yammera REST.

**Exportovať**

[Exportovanie sieťových údajov v správcovi siete](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) povoľuje export obsahu zo sietí yammera vrátane správ a súborov. Prílohy môžu byť veľmi veľké a budú mať za následok, že vývoz bude mať značný časový význam. Odporúčame, aby sa aktívne siete exportovali pomocou [rozhrania API na export údajov](https://developer.yammer.com/docs/data-export-api) v kúskoch za deň alebo týždeň. Technická podpora spoločnosti Microsoft neposkytuje na tento účel vlastné skripty.

Na exportovanie obsahu pre jednotlivých používateľov existuje samostatný [HDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) .