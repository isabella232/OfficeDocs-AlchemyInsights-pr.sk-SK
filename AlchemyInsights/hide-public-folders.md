---
title: Skrytie verejných priečinkov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315439"
---
# <a name="hide-public-folders"></a>Skrytie verejných priečinkov

**Skrytie celého verejného stromu priečinkov**:

Pomocou krokov v [tomto](https://aka.ms/ControlPF) článku skryjete celý verejný strom priečinkov od selektívnych alebo všetkých používateľov.

**Skrytie konkrétneho verejného priečinka**:

1. Pridanie povolení pre používateľov, ktorí potrebujú prístup k verejnému priečinku

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Odstránenie **predvoleného** používateľa zo zoznamu **povolení** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
