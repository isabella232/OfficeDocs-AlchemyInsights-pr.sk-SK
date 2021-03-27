---
title: Pokročilé koncepcie overovania platné pre Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398600"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="56e64-102">Pokročilé koncepcie overovania platné pre Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="56e64-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="56e64-103">Nižšie sú uvedené pokročilé koncepty overovania, ktoré sa vzťahujú na Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="56e64-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="56e64-104">**Proaktívne overovanie**</span><span class="sxs-lookup"><span data-stu-id="56e64-104">**Proactive Authentication**</span></span>

<span data-ttu-id="56e64-105">Po zapnutí politiky [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) sa Microsoft Edge pokúsi proaktívne overiť prihlásených používateľov prostredníctvom služieb spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="56e64-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="56e64-106">V pravidelných intervaloch bude používať online službu na kontrolu aktualizovaného manifestu, ktorý obsahuje konfiguráciu, ktorá riadi proaktívne overovanie.</span><span class="sxs-lookup"><span data-stu-id="56e64-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="56e64-107">Výhody: Proaktívne overovanie umožňuje overovanie v kľúčových službách, ako je napríklad stránka Nová karta balíka Office.</span><span class="sxs-lookup"><span data-stu-id="56e64-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="56e64-108">Ak sa ako vyhľadávací nástroj používa Bing, proaktívne overovanie zlepšuje výkon panela s adresou a pomáha generovať výsledky vyhľadávania prispôsobené potrebám vášho podniku.</span><span class="sxs-lookup"><span data-stu-id="56e64-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="56e64-109">**Overovanie Systému Windows Hello CredUI pre systém NTLM**</span><span class="sxs-lookup"><span data-stu-id="56e64-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="56e64-110">Ak jediné prihlásenie (SSO) nie je k dispozícii, keď sa webová lokalita pokúsi používateľa prihlásiť prostredníctvom mechanizmu NTLM alebo Vyjednať, táto funkcia umožní používateľovi zdieľať poverenia operačného systému s webovou lokalitu a splniť výzvu overenia pomocou používateľského rozhrania Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="56e64-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="56e64-111">Tento tok prihlásenia sa zobrazí len vo Windowse 10 a len pre používateľov, ktorí nemajú jediné prihlásenie počas NTLM alebo vyjednania výzvu Vyjednať.</span><span class="sxs-lookup"><span data-stu-id="56e64-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="56e64-112">**Automatické prihlásenie pomocou uložených hesiel**</span><span class="sxs-lookup"><span data-stu-id="56e64-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="56e64-113">Používatelia, ktorí ukladajú heslá v Microsoft Edgei, môžu povoliť automatické prihlásenie na webové lokality, na ktorých uložili poverenia.</span><span class="sxs-lookup"><span data-stu-id="56e64-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="56e64-114">Používatelia môžu túto funkciu v počítačovej edge://settings/passwords zapnúť alebo vypnúť a môžete ju nakonfigurovať v rámci politík [správcu hesiel.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="56e64-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
