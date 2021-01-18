---
title: Virtuálna konfigurácia s doménovou službou AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885649"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="b0be2-102">Virtuálna konfigurácia s doménovou službou AAD</span><span class="sxs-lookup"><span data-stu-id="b0be2-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="b0be2-103">Virtuálna konfigurácia s doménovou službou AAD zahŕňa tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="b0be2-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="b0be2-104">Kontrola stavu domény na portáli Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="b0be2-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="b0be2-105">Kontrola NSG pravidiel, ktoré blokujú porty potrebné na synchronizáciu v službe Azure AD Domain Services na portáli https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="b0be2-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="b0be2-106">Zabezpečte, aby bola Vaša virtuálna sieť nasadená v rovnakej oblasti Azure ako doména spravovaná doménou služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0be2-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="b0be2-107">Zabezpečte, že nemáte existujúcu doménu s rovnakým názvom domény, ktorá je k dispozícii vo virtuálnej sieti.</span><span class="sxs-lookup"><span data-stu-id="b0be2-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="b0be2-108">Ďalšie informácie o návrhu v službe Azure Virtual Network na podporu doménových služieb AAD nájdete v téme [virtuálna sieť úvaha](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="b0be2-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

