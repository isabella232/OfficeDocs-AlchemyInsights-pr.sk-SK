---
title: Automatické presúvanie e-mailových správ do archívnej poštovej schránky
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749288"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="95f2c-102">Automatické presúvanie e-mailových správ do archívnej poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="95f2c-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="95f2c-103">Tu je postup, ako nastaviť politiku na automatické premiestnenie starého e-mailu používateľa do archívnej poštovej schránky:</span><span class="sxs-lookup"><span data-stu-id="95f2c-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="95f2c-104">Prejdite na položky [**zabezpečenie & súladu s predpismi**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  na **správu údajov**  >   a overte, či je pre používateľa povolená archivácia poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="95f2c-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="95f2c-105">Ak nie, kliknite na položku **Povoliť** a potom v poli upozornenie na tlačidlo **Áno** .</span><span class="sxs-lookup"><span data-stu-id="95f2c-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="95f2c-106">Prejdite do centra spravovania pre [**Exchange > spravovanie súladu > značky uchovávania údajov**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="95f2c-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="95f2c-107">Vyberte ikonu + a potom vyberte položku **automaticky použiť na celú poštovú schránku**.</span><span class="sxs-lookup"><span data-stu-id="95f2c-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="95f2c-108">Priraďte názov značky uchovávania údajov a vyberte položku **premiestniť do archívu**.</span><span class="sxs-lookup"><span data-stu-id="95f2c-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="95f2c-109">Pre obdobie uchovávania údajov zadajte požadovaný čas, napríklad 90 dní.</span><span class="sxs-lookup"><span data-stu-id="95f2c-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="95f2c-110">Kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="95f2c-110">Click **Save**.</span></span>
5. <span data-ttu-id="95f2c-111">Teraz vytvorte politiku uchovávania údajov: vyberte položku **politiky uchovávania údajov**, vyberte ikonu, ak chcete pridať novú politiku.</span><span class="sxs-lookup"><span data-stu-id="95f2c-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="95f2c-112">Priraďte názov k politike uchovávania údajov, potom kliknutím a posunutím vyhľadajte a pridajte značku uchovávania údajov, ktorú ste práve vytvorili.</span><span class="sxs-lookup"><span data-stu-id="95f2c-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="95f2c-113">Kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="95f2c-113">Click **Save**.</span></span>
7. <span data-ttu-id="95f2c-114">Nakoniec použite politiku uchovávania údajov v poštovej schránke používateľa: stále v centre spravovania pre Exchange prejdite na položku  >  **poštové schránky** príjemcov.</span><span class="sxs-lookup"><span data-stu-id="95f2c-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="95f2c-115">Vyberte všetkých používateľov, s ktorými chcete politiku použiť, a potom vyberte položku **Upraviť** (ikona ceruzky).</span><span class="sxs-lookup"><span data-stu-id="95f2c-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="95f2c-116">V dialógovom okne kliknite na položku **funkcie poštovej schránky**.</span><span class="sxs-lookup"><span data-stu-id="95f2c-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="95f2c-117">V časti **politika uchovávania údajov** použite politiku, ktorú ste práve vytvorili > **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="95f2c-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="95f2c-118">Pokyny na použitie politiky pre všetkých používateľov nájdete v téme [Použitie politiky uchovávania údajov v poštových schránkach](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="95f2c-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
