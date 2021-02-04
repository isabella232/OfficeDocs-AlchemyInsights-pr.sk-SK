---
title: Aktivácia spätného zápisu hesiel v službe Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093370"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="5592e-102">Aktivácia spätného zápisu hesiel v službe Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="5592e-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="5592e-103">Ak chcete aktivovať spätný zápis samoobslužného resetovania hesla, najskôr aktivujte v službe Azure AD Connect možnosť spätného zápisu.</span><span class="sxs-lookup"><span data-stu-id="5592e-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="5592e-104">Na serveri Azure AD Connect vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="5592e-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="5592e-105">Prihláste sa na serveri Azure AD Connect a spustite sprievodcu konfiguráciou služby **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="5592e-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="5592e-106">Na stránke **Welcome** (Vitajte) kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="5592e-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="5592e-107">Na stránke **Additional tasks** (Ďalšie úlohy) vyberte možnosť **Customize synchronization options** (Prispôsobiť možnosti synchronizácie) a kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="5592e-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="5592e-108">Na stránke **Connect to Azure AD** (Pripojenie k službe AAD) zadajte prihlasovacie údaje globálneho správcu pre nájomníka platformy Azure a kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="5592e-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="5592e-109">Na stránkach **Connect directories** (Pripojenie adresárov) a **Domain/OU filtering** (Filtrovanie domén/organizačných jednotiek) kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="5592e-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="5592e-110">Na stránke **Optional features** (Voliteľné funkcie) začiarknite políčko vedľa možnosti **Password writeback** (Spätný zápis hesiel) a kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="5592e-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="5592e-111">Na stránke **Ready to configure** (Pripravené na konfiguráciu) kliknite na položku **Configure** (Konfigurovať) a počkajte na dokončenie procesu.</span><span class="sxs-lookup"><span data-stu-id="5592e-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="5592e-112">Keď uvidíte, že sa konfigurácia dokončila, kliknite na možnosť **Exit** (Ukončiť).</span><span class="sxs-lookup"><span data-stu-id="5592e-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="5592e-113">Keď máte v službe Azure AD Connect aktivovaný spätný zápis hesiel, nakonfigurujte na spätný zápis Azure AD SSPR.</span><span class="sxs-lookup"><span data-stu-id="5592e-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="5592e-114">Ak chcete aktivovať spätný zápis hesiel v službe SSPR, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="5592e-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="5592e-115">Prihláste sa na portáli Azure použitím konta globálneho správcu.</span><span class="sxs-lookup"><span data-stu-id="5592e-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="5592e-116">Vyhľadajte a vyberte možnosť **Azure Active Directory**, kliknite na položku **Password reset** (Resetovať heslo) a potom na možnosť **On-premises integration** (Lokálna integrácia).</span><span class="sxs-lookup"><span data-stu-id="5592e-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="5592e-117">Možnosť **Write back passwords to your on-premises directory?** (Zapisovať heslá spätne do lokálneho adresára?) nastavte na **Yes** (Áno).</span><span class="sxs-lookup"><span data-stu-id="5592e-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="5592e-118">Možnosť **Allow users to unlock accounts without resetting their password?** (Povoliť používateľom odomykať kontá bez resetovania hesiel?) nastavte na **Yes** (Áno).</span><span class="sxs-lookup"><span data-stu-id="5592e-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="5592e-119">Keď bude všetko pripravené, kliknite na položku **Save** (Uložiť).</span><span class="sxs-lookup"><span data-stu-id="5592e-119">When ready, click **Save**.</span></span>

<span data-ttu-id="5592e-120">Ďalšie informácie nájdete v téme [Aktivácia spätného zápisu samoobslužného resetovania hesla v službe Azure Active Directory v lokálnom prostredí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="5592e-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="5592e-121">Keď správca resetuje heslo používateľa na portáli Azure a daný používateľ je externý alebo má synchronizovanú hodnotu hash hesla, heslo sa v lokálnom systéme spätne zapíše.</span><span class="sxs-lookup"><span data-stu-id="5592e-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="5592e-122">Táto funkcia vyžaduje licenciu Azure Premium (P1 alebo P2) a aktuálne ju portál Office Admin nepodporuje</span><span class="sxs-lookup"><span data-stu-id="5592e-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
