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
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939934"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Riešenie problémov s pripojením k službe Azure AD

1. Ak nastavujete registráciu zariadenia po prvýkrát, uistite sa, že ste si už v spoločnosti Azure Active Directory prešli úvod do správy [zariadení,](https://docs.microsoft.com/azure/active-directory/devices/overview) kde nájdete postup, ako získať zariadenia pod kontrolou na Azure AD. 
1. Ak svoje zariadenia zaregistrujete priamo v službe Azure AD a zaregistrujete ich do služby Intune, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) musíte sa najskôr ubezpečiť, že ste nakonfigurovali [službu Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) a že licencie máte nastavené.
1. Uistite sa, že máte oprávnenie vykonávať operácie v službe Azure AD. Nastavenia registrácií zariadení môže spravovať iba globálny správca v službe Azure AD.
1. Informácie o implementácii spojenia so službou Azure AD nájdete v [téme Plánovanie pripájanie k službe Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Ďalšie informácie o riešení bežných problémov s pripojením k službe Azure AD nájdete v téme Najčastejšie otázky týkajúce sa služby [Azure Ad a](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) pre Windows 10 Pro zariadenie nájdete v téme Nepodarilo sa pripojiť k počítaču Windows 10 Pro so službou Azure AD – je potrebné vykonať inováciu na – [komunita Microsoft](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
