---
title: Problém s otváraním alebo preberaním súborov v Yammeri
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
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148340"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="87ae4-102">Problém s otváraním alebo preberaním súborov v Yammeri</span><span class="sxs-lookup"><span data-stu-id="87ae4-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="87ae4-103">Classic Yammer podporuje viaceré možnosti pre odovzdávanie súborov do správ a skupín.</span><span class="sxs-lookup"><span data-stu-id="87ae4-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="87ae4-104">V závislosti od konfigurácie siete sú súbory predvolené pre ukladanie v SharePointe.</span><span class="sxs-lookup"><span data-stu-id="87ae4-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="87ae4-105">Výber súborov v novom nariekanie zatiaľ nepodporuje všetky možnosti dostupné v klasickom nariekanie.</span><span class="sxs-lookup"><span data-stu-id="87ae4-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="87ae4-106">Budúca aktualizácia pridá ďalšie funkcie.</span><span class="sxs-lookup"><span data-stu-id="87ae4-106">A future update will add additional features.</span></span> <span data-ttu-id="87ae4-107">Ďalšie informácie nájdete v téme [Priloženie súboru alebo obrázka k príspevku konverzácie yammera](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="87ae4-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="87ae4-108">**Súbor sa nedá otvoriť alebo prevziať**</span><span class="sxs-lookup"><span data-stu-id="87ae4-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="87ae4-109">Súbor sa môže nahrať do yammera, ale aj prepojenie na súbor v SharePointe Online.</span><span class="sxs-lookup"><span data-stu-id="87ae4-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="87ae4-110">Ak chcete riešiť problémy, najprv musíte určiť umiestnenie súboru.</span><span class="sxs-lookup"><span data-stu-id="87ae4-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="87ae4-111">Ak bol súbor odovzdaný na sieť Yammer, bude mať adresu URL \*.yammer.com.</span><span class="sxs-lookup"><span data-stu-id="87ae4-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="87ae4-112">Skontrolujte, či sú požadované adresy URL a adresy IP odblokované.</span><span class="sxs-lookup"><span data-stu-id="87ae4-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="87ae4-113">Ďalšie informácie nájdete v blogovom príspevku [Používanie pevných kódovaných adries IP pre yammer sa neodporúča](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="87ae4-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="87ae4-114">Skontrolujte, či používateľ, ktorý je tiež globálnym správcom, môže súbor prevziať.</span><span class="sxs-lookup"><span data-stu-id="87ae4-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="87ae4-115">Ak je súbor súkromný, možno budete musieť použiť režim súkromného obsahu.</span><span class="sxs-lookup"><span data-stu-id="87ae4-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="87ae4-116">Ďalšie informácie nájdete v téme [Sledovanie súkromného obsahu v yammeri](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="87ae4-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="87ae4-117">**Hostia a súbory na úrovni siete Yammer v SharePointe Online**</span><span class="sxs-lookup"><span data-stu-id="87ae4-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="87ae4-118">[Na úrovni siete na úrovni siete Nariekanie](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nepoužívajte Azure AD B2B a sú interné nariekanie služby, takže nemajú prístup k súborom yammer uložené v SharePoint.</span><span class="sxs-lookup"><span data-stu-id="87ae4-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="87ae4-119">Vytvorte externéHo používateľa AAD B2B, ktorý má prístup ku knižniciam dokumentov v SharePointe Online pomocou tejto identity.</span><span class="sxs-lookup"><span data-stu-id="87ae4-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="87ae4-120">Informácie o budúcej podpore hosťových hostí služby Azure AD B2B v Yammeri nájdete v téme [Podpora pre hostí spoločnosti Business-to-business (B2B) v téme Ukážka služby Yammer – podmienky pre zákazníka a najčastejšie otázky](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="87ae4-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>