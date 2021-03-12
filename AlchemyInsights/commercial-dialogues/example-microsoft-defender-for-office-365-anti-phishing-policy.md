---
title: Príklad Microsoft Defendera pre Office 365 anti-phishing Policy
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
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750796"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="33109-102">Príklad Microsoft Defendera pre Office 365 anti-phishing Policy</span><span class="sxs-lookup"><span data-stu-id="33109-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="33109-103">Tieto nastavenia umožňujú politiku s názvom *domain and CEO*.</span><span class="sxs-lookup"><span data-stu-id="33109-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="33109-104">Táto politika poskytuje ochranu používateľov aj domény pred zosobnením a potom použije politiku na všetky e-maily prijaté používateľmi v rámci domény.</span><span class="sxs-lookup"><span data-stu-id="33109-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="33109-105">Najprv pridajte nasledujúce informácie na vytvorenie politiky:</span><span class="sxs-lookup"><span data-stu-id="33109-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="33109-106">**Názov**: Domain and CEO **Popis**: zabezpečuje, že generálny riaditeľ a vaša doména nie sú zosobnené.</span><span class="sxs-lookup"><span data-stu-id="33109-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="33109-107">**Použiť na**: vyberte **doménu príjemcu**.</span><span class="sxs-lookup"><span data-stu-id="33109-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="33109-108">V časti **niektoré z týchto** vyberte položku **vybrať** a potom vyberte doménu.</span><span class="sxs-lookup"><span data-stu-id="33109-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="33109-109">Vyberte položku **+ Pridať**.</span><span class="sxs-lookup"><span data-stu-id="33109-109">Select **+ Add**.</span></span> <span data-ttu-id="33109-110">Začiarknite políčko vedľa názvu domény v zozname (napríklad *contoso.com*) a potom vyberte položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="33109-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="33109-111">Vyberte položku **Hotovo**.</span><span class="sxs-lookup"><span data-stu-id="33109-111">Select **Done**.</span></span>
- <span data-ttu-id="33109-112">Po vytvorení politiky môžete politiku jemne doladiť pomocou nasledujúcich možností:</span><span class="sxs-lookup"><span data-stu-id="33109-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="33109-113">**Pridanie používateľov na ochranu:** V tomto príklade pridajte e-mailovú adresu CEO na minimum.</span><span class="sxs-lookup"><span data-stu-id="33109-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="33109-114">**Pridanie domén na ochranu**: Pridajte organizačnú doménu, ktorá obsahuje kanceláriu generálneho riaditeľa.</span><span class="sxs-lookup"><span data-stu-id="33109-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="33109-115">**Vyberte položku akcie**: v **prípade odoslania e-mailu prostredníctvom zosobneného používateľa** vyberte položku **presmerovať správu na inú e-mailovú adresu** a potom zadajte e-mailovú adresu správcu zabezpečenia (napríklad *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="33109-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="33109-116">**Ak je e-mail odoslaný** vybratou doménou, vyberte položku **karanténa správy**.</span><span class="sxs-lookup"><span data-stu-id="33109-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="33109-117">**Poštová schránka inteligencia**: Táto možnosť je predvolene vybratá pri vytváraní novej politiky ochrany pred neoprávneným získavaním údajov.</span><span class="sxs-lookup"><span data-stu-id="33109-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="33109-118">Ak chcete najlepšie výsledky, nechajte toto nastavenie **zapnuté** .</span><span class="sxs-lookup"><span data-stu-id="33109-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="33109-119">**Pridanie dôveryhodných odosielateľov a domén:** V tomto príklade nedefinujte žiadne prepíše.</span><span class="sxs-lookup"><span data-stu-id="33109-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="33109-120">Po skontrolovaní nastavení vyberte v prípade potreby položku **vytvoriť túto politiku** alebo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="33109-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="33109-121">Ďalšie informácie nájdete v téme [politiky ochrany pred neoprávneným získavaním údajov v Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="33109-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
