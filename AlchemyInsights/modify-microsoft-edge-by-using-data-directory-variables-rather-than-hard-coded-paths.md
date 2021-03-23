---
title: Úprava Microsoft Edge pomocou premenných adresára údajov namiesto pevných nakódovaných ciest
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036856"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Úprava Microsoft Edge pomocou premenných adresára údajov namiesto pevných nakódovaných ciest

Ak chcete napríklad v systéme Windows uložiť údaje profilu v rámci miestnych údajov aplikácie používateľa namiesto v predvolenom umiestnení, nastavte politiku *UserDataDir* na hodnotu **$ {local_app_data} \Edge\Profile**.

Ďalšie informácie nájdete v téme [Vytvorenie premenných adresárov používateľských údajov v prehliadači Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).