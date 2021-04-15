---
title: Chyba aplikácie Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786684"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="205bc-102">Chyba 4c7 v aplikácii Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="205bc-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="205bc-103">Táto chyba sa vyskytuje, pretože aplikácia Microsoft Teams vyžaduje overovanie formulárov.</span><span class="sxs-lookup"><span data-stu-id="205bc-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="205bc-104">Keď nasadzujete Active Directory Federation Services (ADFS), overovanie formulárov nie je predvolene povolené pre intranet.</span><span class="sxs-lookup"><span data-stu-id="205bc-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="205bc-105">Ak integrované overovanie systému Windows zlyhá, zobrazí sa výzva na prihlásenie pomocou overenia formulárov.</span><span class="sxs-lookup"><span data-stu-id="205bc-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="205bc-106">Ak chcete tento problém vyriešiť, povoľte overovanie formulárov pomocou modulu Microsoft Management Console (MMC) služby ADFS v počítači, ktorý obsahuje lokálnu kópiu služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="205bc-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="205bc-107">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="205bc-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="205bc-108">Na navigačnej table prejdite na položku **Politiky overovania.**</span><span class="sxs-lookup"><span data-stu-id="205bc-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="205bc-109">V **časti Akcie** na table s podrobnosťami vyberte položku Upraviť globálne primárne **overovanie**.</span><span class="sxs-lookup"><span data-stu-id="205bc-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="205bc-110">Na karte **Intranet** vyberte položku **Overovanie formulárov.**</span><span class="sxs-lookup"><span data-stu-id="205bc-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="205bc-111">Vyberte **tlačidlo OK** (alebo **Použiť**).</span><span class="sxs-lookup"><span data-stu-id="205bc-111">Select **OK** (or **Apply**).</span></span>