---
title: Riešenie problémov s pripojením k službe Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405760"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Riešenie problémov s pripojením k službe Azure AD

1. Ak nastavujete registráciu zariadenia po prvýkrát, uistite sa, že ste si už preskúmali úvodné informácie o riadení zariadení v [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) kde nájdete postup, ako získať zariadenia pod kontrolou na Azure AD. 
1. Ak svoje zariadenia zaregistrujete priamo v službe Azure AD a zaregistrujete ich do služby Intune, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) musíte sa najskôr ubezpečiť, že ste nakonfigurovali [službu Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) a že licencie máte nastavené.
1. Uistite sa, že máte oprávnenie vykonávať operácie v službe Azure AD. Nastavenia registrácií zariadenia môže spravovať iba globálny správca v službe Azure AD.
1. Informácie o implementácii spojenia so službou Azure AD nájdete v [téme Plánovanie pripájanie k službe Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Ďalšie informácie o riešení bežných problémov s pripojením k službe Azure AD nájdete v téme Najčastejšie otázky týkajúce sa služby [Azure Ad a](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) pre zariadenie s Windowsom 10 Pro. Pozrite si článok Nedá sa pripojiť k počítaču s [Windowsom 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) k službe Azure AD – je potrebné inovovať na – komunita Microsoft
