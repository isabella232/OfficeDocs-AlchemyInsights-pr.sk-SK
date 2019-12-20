---
title: Tímy 4c 7 chyba
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796360"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="b4342-102">4c 7 chyba v Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="b4342-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="b4342-103">Táto chyba sa vyskytuje, pretože Microsoft teams vyžaduje overovanie formulárov.</span><span class="sxs-lookup"><span data-stu-id="b4342-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="b4342-104">Pri nasadzovaní služby Active Directory Federation Services (AD FS), overovanie formulárov nie je povolená pre intranet predvolene.</span><span class="sxs-lookup"><span data-stu-id="b4342-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="b4342-105">Ak Windows integrované overovanie zlyhá, sa zobrazí výzva na prihlásenie pomocou overovanie formulárov.</span><span class="sxs-lookup"><span data-stu-id="b4342-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="b4342-106">Ak chcete vyriešiť tento problém, povoľte overovanie formulárov pomocou modulu AD FS Microsoft Management Console (MMC) v počítači, ktorý má lokálnu kópiu služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b4342-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="b4342-107">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="b4342-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="b4342-108">Na navigačnej table prejdite na položku **politiky overovania**.</span><span class="sxs-lookup"><span data-stu-id="b4342-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="b4342-109">V časti **akcie** na table s podrobnosťami vyberte položku **Upraviť globálne primárne overovanie**.</span><span class="sxs-lookup"><span data-stu-id="b4342-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="b4342-110">Na karte **intranet** vyberte **overovanie formulárov**.</span><span class="sxs-lookup"><span data-stu-id="b4342-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="b4342-111">Vyberte položku **OK** (alebo **aplikovať**).</span><span class="sxs-lookup"><span data-stu-id="b4342-111">Select **OK** (or **Apply**).</span></span>