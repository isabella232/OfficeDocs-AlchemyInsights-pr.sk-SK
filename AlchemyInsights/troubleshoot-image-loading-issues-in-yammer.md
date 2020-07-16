---
title: Riešenie problémov s načítaním obrázkov v Yammeri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148298"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="91797-102">Riešenie problémov s načítaním obrázkov v Yammeri</span><span class="sxs-lookup"><span data-stu-id="91797-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="91797-103">Keď sa vyskytnú problémy s fotografiami a ukážky súborov v sieti Yammer, riešenie problémov kontrolou, či sa problém vyskytuje pre všetkých používateľov, či sa vyskytuje na mobilných zariadeniach, a ak je reprodukovateľný pri nahrávaní prílohy.</span><span class="sxs-lookup"><span data-stu-id="91797-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="91797-104">**Problémy s profilovou fotografiou**</span><span class="sxs-lookup"><span data-stu-id="91797-104">**Profile photo issues**</span></span>  

<span data-ttu-id="91797-105">Ak sa koncoví používatelia prihlásia do yammera cez Microsoft 365, musia zmeniť svoj profil vrátane ich profilovej fotografie.</span><span class="sxs-lookup"><span data-stu-id="91797-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="91797-106">Ak používatelia nie sú povolené vykonávať aktualizácie profilu, správca môže vykonať aktualizáciu pre používateľa.</span><span class="sxs-lookup"><span data-stu-id="91797-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="91797-107">Ďalšie informácie nájdete v téme [Zobrazenie a aktualizácia profilu v Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="91797-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="91797-108">Informácie o úprave profilu vrátane profilovej fotografie nájdete v téme [Zmena profilu a nastavení yammera](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="91797-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="91797-109">Aktualizované profilové fotografie sa synchronizujú inak ako atribúty profilu.</span><span class="sxs-lookup"><span data-stu-id="91797-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="91797-110">Používatelia sa musia prihlásiť, aby spustili synchronizáciu svojej profilovej fotografie.</span><span class="sxs-lookup"><span data-stu-id="91797-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="91797-111">Informácie nájdete v téme [Sú obrázky používateľského profilu aktualizované zo služieb Office 365 na Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="91797-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="91797-112">Informácie o životnom cykle používateľa yammera nájdete v téme [Správa používateľov Yammera počas ich životného cyklu zo služieb Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="91797-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="91797-113">Podrobnosti o fungovaní synchronizácie obrázkov profilu v službe Microsoft 365 nájdete v téme [Informácie o synchronizácii profilov ej synchronizácie s obrázkami v službe Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="91797-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="91797-114">**Ukážky dokumentov a problémy s miniatúrami obrázkov**</span><span class="sxs-lookup"><span data-stu-id="91797-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="91797-115">Keď sa súbory alebo obrázky zaverejňujú do yammera, ukážky sa nemusia zobraziť, pretože:</span><span class="sxs-lookup"><span data-stu-id="91797-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="91797-116">Súbor je poškodený a nedá sa spracovať.</span><span class="sxs-lookup"><span data-stu-id="91797-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="91797-117">Súbor nebol nedávno odovzdaný do SharePointu Online alebo sieť Yammer obsahuje neplatné metaúdaje z iných dôvodov.</span><span class="sxs-lookup"><span data-stu-id="91797-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="91797-118">Adresy URL potrebné na načítanie obrázkov s ukážkou sú blokované.</span><span class="sxs-lookup"><span data-stu-id="91797-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="91797-119">Pred odoslaním používateľ odstránil ukážku súboru.</span><span class="sxs-lookup"><span data-stu-id="91797-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="91797-120">Problém so službou zabránil vygenerovaniu ukážky.</span><span class="sxs-lookup"><span data-stu-id="91797-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="91797-121">**Upozornenie:** Ukážky prepojení a odovzdávania súborov sa môžu správať inak.</span><span class="sxs-lookup"><span data-stu-id="91797-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="91797-122">Prepojenia na súbory na internete alebo prepojenia, ktoré vyžadujú ďalšie overovanie, sa nemusia zobraziť správne.</span><span class="sxs-lookup"><span data-stu-id="91797-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="91797-123">Ďalšie informácie nájdete v téme [Priloženie súboru alebo obrázka k správe yammera](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="91797-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 