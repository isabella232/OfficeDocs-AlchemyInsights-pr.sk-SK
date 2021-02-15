---
title: Heslo zápisom nefunguje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243522"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="a5ad7-102">Heslo zápisom nefunguje</span><span class="sxs-lookup"><span data-stu-id="a5ad7-102">Password Writeback is not working</span></span>

<span data-ttu-id="a5ad7-103">**Mám problémy s konfiguráciou hesla zápisom**</span><span class="sxs-lookup"><span data-stu-id="a5ad7-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="a5ad7-104">Funkcia Password zápisom je prémiovou funkciou.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="a5ad7-105">Uistite sa, že chápete licenčné požiadavky:</span><span class="sxs-lookup"><span data-stu-id="a5ad7-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="a5ad7-106">V organizácii musíte mať priradenú aspoň jednu licenciu.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="a5ad7-107">**Iba používatelia cloudu** – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="a5ad7-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="a5ad7-108">**Cloudové a/alebo lokálne používatelia** – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)</span><span class="sxs-lookup"><span data-stu-id="a5ad7-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="a5ad7-109">Ďalšie informácie o licenčných požiadavkách nájdete [v téme licenčné požiadavky na vytvorenie nového hesla služby Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="a5ad7-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="a5ad7-110">Máte aspoň jedno konto správcu a jedno skúšobné používateľské konto s jednou z príslušných licencií.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="a5ad7-111">Pripojenie Azure AD sa musí pripojiť k primárnemu emulátoru radiča domény na zápisom hesla.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="a5ad7-112">Azure AD Connect môžete nakonfigurovať tak, aby používal primárny radič domény kliknutím pravým tlačidlom myši na **Vlastnosti** konektora synchronizácie služby Active Directory a potom vyberte položku **konfigurovať oblasti adresárov**.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="a5ad7-113">Pozrite si časť **Nastavenie pripojenia radiča domény** a začiarknite políčko s názvom **iba preferované radiče domén**.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="a5ad7-114">Ak prednostné DC nie je emulátorom PDC, Azure AD Connect bude stále osloviť PDC pre heslo zápisom.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="a5ad7-115">Obnovenie hesla bolo nakonfigurované a povolené v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="a5ad7-116">Ďalšie informácie nájdete v téme [Povolenie používateľom obnoviť svoje heslá v službe Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="a5ad7-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="a5ad7-117">Uistite sa, že konto správcu používané na povolenie hesla zápisom je kontom správcu cloudu (vytvorené v službe Azure AD nie lokálneho AD)</span><span class="sxs-lookup"><span data-stu-id="a5ad7-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="a5ad7-118">Máte jedno alebo viaceré lesné AD lokálne nasadenie so systémom Windows Server 2008 R2, Windows Server 2012 alebo Windows Server 2012 R2 s nainštalovanými najnovšími balíkmi Service Pack</span><span class="sxs-lookup"><span data-stu-id="a5ad7-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="a5ad7-119">Máte nainštalovaný nástroj Azure AD Connect a máte pripravené prostredie na synchronizáciu v cloude.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="a5ad7-120">Pred vykonaním testovania hesla zápisom Skontrolujte, či ste najprv dokončili úplný import a úplnú synchronizáciu zo služby AD a Azure AD v službe Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a5ad7-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="a5ad7-121">Ďalšie informácie nájdete v téme postup pri [úplnej synchronizácii a úplnom importovaní v službe Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="a5ad7-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="a5ad7-122">**Mám problém s pripojením hesla zápisom**</span><span class="sxs-lookup"><span data-stu-id="a5ad7-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="a5ad7-123">Stiahnutie a povolenie najnovšej verzie služby [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="a5ad7-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="a5ad7-124">Konfigurácia brány firewall: nástroj Azure AD Connect (1.1.443 a novší) bude potrebovať **ODCHÁDZAJÚCE https** prístup k:</span><span class="sxs-lookup"><span data-stu-id="a5ad7-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="a5ad7-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a5ad7-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="a5ad7-126">ServiceBus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="a5ad7-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="a5ad7-127">Povolenie nečinných pripojení trvá minimálne 2-3 minút</span><span class="sxs-lookup"><span data-stu-id="a5ad7-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="a5ad7-128">**Stále mám problémy s heslom zápisom**</span><span class="sxs-lookup"><span data-stu-id="a5ad7-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="a5ad7-129">Ak problémy pretrvávajú, skúste vypnúť a znova zapnúť službu Password zápisom v nástroji Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="a5ad7-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="a5ad7-130">Ďalšie informácie nájdete v téme [Vypnutie a opätovné zapnutie hesla zápisom](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="a5ad7-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
