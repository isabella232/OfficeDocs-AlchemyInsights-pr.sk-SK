---
title: Konfigurovanie bodu pripojenia služby (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037288"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="06366-102">Konfigurovanie bodu pripojenia služby (SCP)</span><span class="sxs-lookup"><span data-stu-id="06366-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="06366-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="06366-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="06366-104">**Dôvod**: nie je možné prečítať objekt SCP a získať informácie o nájomníkovi služby Azure AD</span><span class="sxs-lookup"><span data-stu-id="06366-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="06366-105">**Riešenie**: Prečítajte si časť [Konfigurácia bodu pripojenia služby](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="06366-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="06366-106">**Akčný plán**</span><span class="sxs-lookup"><span data-stu-id="06366-106">**Action plan**</span></span>

- <span data-ttu-id="06366-107">Skontrolujte, či zariadenie prijalo objekt GPO na kontrolované overenie.</span><span class="sxs-lookup"><span data-stu-id="06366-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="06366-108">Presvedčte sa, že objekt GPO vytvoril kľúče databázy Registry.</span><span class="sxs-lookup"><span data-stu-id="06366-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="06366-109">Uistite sa, že máte 2 kľúče vytvorené pomocou IDENTIFIKÁTORa adresára a domény onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="06366-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="06366-110">**Konfigurácia nastavenia databázy Registry na strane klienta pre SCP**</span><span class="sxs-lookup"><span data-stu-id="06366-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="06366-111">Použite nasledujúci príklad na vytvorenie objektu skupinovej politiky (GPO) na nasadenie nastavenia databázy Registry, ktoré konfiguruje položku SCP v databáze Registry svojich zariadení.</span><span class="sxs-lookup"><span data-stu-id="06366-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="06366-112">Otvorte konzolu na správu skupinovej politiky a vytvorte nový objekt GPO v doméne.</span><span class="sxs-lookup"><span data-stu-id="06366-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="06366-113">Poskytnite svoj novovytvorený objekt GPO názov (napríklad ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="06366-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="06366-114">Upravte objekt GPO a vyhľadajte nasledujúcu cestu: **Konfigurácia počítača > predvoľby > nastavenie systému Windows > Registry**.</span><span class="sxs-lookup"><span data-stu-id="06366-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="06366-115">Kliknite pravým tlačidlom myši na **databázu Registry** a vyberte položku **Nová položka databázy Registry >**.</span><span class="sxs-lookup"><span data-stu-id="06366-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="06366-116">Na karte **Všeobecné** nakonfigurujte nasledovné:</span><span class="sxs-lookup"><span data-stu-id="06366-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="06366-117">**Akcia**: Aktualizácia</span><span class="sxs-lookup"><span data-stu-id="06366-117">**Action**: Update</span></span>
    
- <span data-ttu-id="06366-118">**Úľ**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="06366-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="06366-119">**Cesta ku kľúču**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="06366-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="06366-120">**Názov hodnoty**: nájomníka</span><span class="sxs-lookup"><span data-stu-id="06366-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="06366-121">**Typ hodnoty**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="06366-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="06366-122">**Údaje o hodnote**: identifikátor GUID alebo adresár vašej inštancie služby Azure AD (Táto hodnota sa nachádza na **portáli Azure Portal > azure Active Directory > vlastnosti > ID adresára**)</span><span class="sxs-lookup"><span data-stu-id="06366-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="06366-123">Kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="06366-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="06366-124">Kliknite pravým tlačidlom myši na **databázu Registry** a vyberte položku **Nová položka databázy Registry >**.</span><span class="sxs-lookup"><span data-stu-id="06366-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="06366-125">Na karte **Všeobecné** nakonfigurujte nasledovné:</span><span class="sxs-lookup"><span data-stu-id="06366-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="06366-126">**Akcia**: Aktualizácia</span><span class="sxs-lookup"><span data-stu-id="06366-126">**Action**: Update</span></span>
    
- <span data-ttu-id="06366-127">**Úľ**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="06366-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="06366-128">**Cesta ku kľúču**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="06366-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="06366-129">**Názov hodnoty**: TenantName</span><span class="sxs-lookup"><span data-stu-id="06366-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="06366-130">**Typ hodnoty**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="06366-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="06366-131">**Údaje o hodnote**: názov overeného názvu domény, ak používate externé prostredie, akým je napríklad AD FS.</span><span class="sxs-lookup"><span data-stu-id="06366-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="06366-132">Váš overený názov domény alebo názov domény onmicrosoft.com (napríklad contoso. onmicrosoft). com, ak používate spravované prostredie</span><span class="sxs-lookup"><span data-stu-id="06366-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="06366-133">Kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="06366-133">Click **OK**.</span></span>

7. <span data-ttu-id="06366-134">Zatvorenie editora pre novovytvorený objekt GPO.</span><span class="sxs-lookup"><span data-stu-id="06366-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="06366-135">Prepojiť novovytvorený objekt GPO s požadovanou OU, ktorá obsahuje počítače pripojené k doméne, ktoré patria do kontrolovaného zavádzacieho súboru.</span><span class="sxs-lookup"><span data-stu-id="06366-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="06366-136">Ďalšie informácie nájdete v téme [riadené overovanie hybridného spojenia Azure AD – Azure AD | Dokumenty spoločnosti Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) a  [Riešenie problémov hybridných zariadení spojených so službou Azure Active Directory | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="06366-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









