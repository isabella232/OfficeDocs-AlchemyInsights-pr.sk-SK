---
title: Importovanie a exportovanie z Yammera
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037259"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="0a0f2-102">Importovanie a exportovanie z Yammera</span><span class="sxs-lookup"><span data-stu-id="0a0f2-102">Import and export from Yammer</span></span>

<span data-ttu-id="0a0f2-103">**Importovať**</span><span class="sxs-lookup"><span data-stu-id="0a0f2-103">**Import**</span></span>

<span data-ttu-id="0a0f2-104">Možnosti importovania používateľov sa líšia v závislosti od toho, či je vaša sieť Yammer v [natívnom režime pre Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)alebo nie.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="0a0f2-105">**Nenatívny režim**: používatelia môžu byť importovaní do skupín pomocou položky [Pridať z adresára](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (obmedziť na 100 používateľov) v rámci nastavenia skupiny alebo do siete s použitím [hromadnej aktualizácie](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) v správcovi siete.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="0a0f2-106">**Natívny režim**: členstvo v skupine a operácie členstva v sieti by sa mali vykonávať na [portáli Microsoft 365 admin Portal](https://docs.microsoft.com/microsoft-365/admin/add-users), v službe [Azure AD Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)alebo pomocou inej možnosti služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="0a0f2-107">Siete v natívnom režime už nemajú prístup k hromadnej aktualizácii a iným starším funkciám.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0a0f2-108">Yammer nikdy nepodporoval Importovanie obsahu v správcovi siete, a to ani v prípade, že funkcia exportu údajov bola použitá v inej sieti.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="0a0f2-109">Obsah môže byť opätovne odoslaný partnerskými riešeniami alebo rozhraniami Yammera REST.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="0a0f2-110">**Exportovať**</span><span class="sxs-lookup"><span data-stu-id="0a0f2-110">**Export**</span></span>

<span data-ttu-id="0a0f2-111">[Exportovanie sieťových údajov v správcovi siete](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) povoľuje export obsahu zo sietí yammera vrátane správ a súborov.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="0a0f2-112">Prílohy môžu byť veľmi veľké a budú mať za následok, že vývoz bude mať značný časový význam.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="0a0f2-113">Odporúčame, aby sa aktívne siete exportovali pomocou [rozhrania API na export údajov](https://developer.yammer.com/docs/data-export-api) v kúskoch za deň alebo týždeň.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="0a0f2-114">Technická podpora spoločnosti Microsoft neposkytuje na tento účel vlastné skripty.</span><span class="sxs-lookup"><span data-stu-id="0a0f2-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="0a0f2-115">Na exportovanie obsahu pre jednotlivých používateľov existuje samostatný [HDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) .</span><span class="sxs-lookup"><span data-stu-id="0a0f2-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>