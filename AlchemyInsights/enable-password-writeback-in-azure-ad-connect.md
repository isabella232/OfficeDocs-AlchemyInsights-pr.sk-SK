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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560455"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="6fb03-102">Aktivácia spätného zápisu hesiel v službe Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="6fb03-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="6fb03-103">Ak chcete aktivovať spätný zápis samoobslužného resetovania hesla, najskôr aktivujte v službe Azure AD Connect možnosť spätného zápisu.</span><span class="sxs-lookup"><span data-stu-id="6fb03-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="6fb03-104">Na serveri Azure AD Connect vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="6fb03-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="6fb03-105">Prihláste sa na serveri Azure AD Connect a spustite sprievodcu konfiguráciou služby **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="6fb03-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="6fb03-106">Na stránke **Welcome** (Vitajte) kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="6fb03-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="6fb03-107">Na stránke **Additional tasks** (Ďalšie úlohy) vyberte možnosť **Customize synchronization options** (Prispôsobiť možnosti synchronizácie) a kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="6fb03-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="6fb03-108">Na stránke **Connect to Azure AD** (Pripojenie k službe AAD) zadajte prihlasovacie údaje globálneho správcu pre nájomníka platformy Azure a kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="6fb03-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="6fb03-109">Na stránkach **Connect directories** (Pripojenie adresárov) a **Domain/OU filtering** (Filtrovanie domén/organizačných jednotiek) kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="6fb03-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="6fb03-110">Na stránke **Optional features** (Voliteľné funkcie) začiarknite políčko vedľa možnosti **Password writeback** (Spätný zápis hesiel) a kliknite na položku **Next** (Ďalej).</span><span class="sxs-lookup"><span data-stu-id="6fb03-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="6fb03-111">Na stránke **Ready to configure** (Pripravené na konfiguráciu) kliknite na položku **Configure** (Konfigurovať) a počkajte na dokončenie procesu.</span><span class="sxs-lookup"><span data-stu-id="6fb03-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="6fb03-112">Keď uvidíte, že sa konfigurácia dokončila, kliknite na možnosť **Exit** (Ukončiť).</span><span class="sxs-lookup"><span data-stu-id="6fb03-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="6fb03-113">Keď máte v službe Azure AD Connect aktivovaný spätný zápis hesiel, nakonfigurujte na spätný zápis Azure AD SSPR.</span><span class="sxs-lookup"><span data-stu-id="6fb03-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="6fb03-114">Ak chcete aktivovať spätný zápis hesiel v službe SSPR, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="6fb03-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="6fb03-115">Prihláste sa na portáli Azure použitím konta globálneho správcu.</span><span class="sxs-lookup"><span data-stu-id="6fb03-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="6fb03-116">Vyhľadajte a vyberte možnosť **Azure Active Directory**, kliknite na položku **Password reset** (Resetovať heslo) a potom na možnosť **On-premises integration** (Lokálna integrácia).</span><span class="sxs-lookup"><span data-stu-id="6fb03-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="6fb03-117">Možnosť **Write back passwords to your on-premises directory?** (Zapisovať heslá spätne do lokálneho adresára?) nastavte na **Yes** (Áno).</span><span class="sxs-lookup"><span data-stu-id="6fb03-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="6fb03-118">Možnosť **Allow users to unlock accounts without resetting their password?** (Povoliť používateľom odomykať kontá bez resetovania hesiel?) nastavte na **Yes** (Áno).</span><span class="sxs-lookup"><span data-stu-id="6fb03-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="6fb03-119">Keď bude všetko pripravené, kliknite na položku **Save** (Uložiť).</span><span class="sxs-lookup"><span data-stu-id="6fb03-119">When ready, click **Save**.</span></span>

<span data-ttu-id="6fb03-120">Ďalšie informácie nájdete v téme [Aktivácia spätného zápisu samoobslužného resetovania hesla v službe Azure Active Directory v lokálnom prostredí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="6fb03-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="6fb03-121">Keď správca resetuje heslo používateľa na portáli Azure a daný používateľ je externý alebo má synchronizovanú hodnotu hash hesla, heslo sa v lokálnom systéme spätne zapíše.</span><span class="sxs-lookup"><span data-stu-id="6fb03-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="6fb03-122">Táto funkcia momentálne nie je na portáli pre správcov balíka Office podporovaná.</span><span class="sxs-lookup"><span data-stu-id="6fb03-122">This functionality is currently not supported in the Office Admin portal.</span></span>