---
title: Rozšírené koncepty overovania platné pre Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573530"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="e3c64-102">Rozšírené koncepty overovania platné pre Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e3c64-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="e3c64-103">Nižšie sú uvedené pokročilé overovacie koncepty, ktoré sa vzťahujú na Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="e3c64-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="e3c64-104">**Proaktívne overovanie**</span><span class="sxs-lookup"><span data-stu-id="e3c64-104">**Proactive Authentication**</span></span>

<span data-ttu-id="e3c64-105">Keď povolíte politiku [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge sa bude pokúšať aktívne autentifikovať používateľov s prihlásením prostredníctvom služieb spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3c64-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="e3c64-106">V pravidelných intervaloch bude používať online službu na vyhľadanie aktualizovaného manifestu, ktorý obsahuje konfiguráciu, ktorá sa riadi proaktívnym overovaním.</span><span class="sxs-lookup"><span data-stu-id="e3c64-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="e3c64-107">Výhody: proaktívne overovanie umožňuje overenie kľúčových služieb, ako je napríklad stránka na novej karte balíka Office.</span><span class="sxs-lookup"><span data-stu-id="e3c64-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="e3c64-108">Aj v prípade, že sa Bing používa ako vyhľadávací nástroj, aktívne overovanie zlepšuje výkon panela s adresou a pomáha vytvárať výsledky vyhľadávania prispôsobené potrebám vášho podniku.</span><span class="sxs-lookup"><span data-stu-id="e3c64-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="e3c64-109">**Windows Hello CredUI pre overovanie NTLM**</span><span class="sxs-lookup"><span data-stu-id="e3c64-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="e3c64-110">Ak nie je k dispozícii jediné prihlásenie (SSO), keď sa webová lokalita pokúsi prihlásiť používateľa prostredníctvom protokolu NTLM alebo vyjednávacieho mechanizmu, táto funkcia umožní používateľovi zdieľať poverenia operačného systému s webovou lokalitou a splniť výzvu na overenie pomocou používateľského rozhrania Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="e3c64-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="e3c64-111">Tento tok pri prihlasovaní sa zobrazí iba vo Windowse 10 a len pre používateľov, ktorí nezískajú SSO v priebehu protokolu NTLM alebo vyjednávacieho problému.</span><span class="sxs-lookup"><span data-stu-id="e3c64-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="e3c64-112">**Automatické prihlásenie pomocou uložených hesiel**</span><span class="sxs-lookup"><span data-stu-id="e3c64-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="e3c64-113">Používatelia, ktorí ukladajú heslá v prehliadači Microsoft Edge, môžu povoliť automatické prihlásenie na webové lokality, na ktorých boli uložené poverenia.</span><span class="sxs-lookup"><span data-stu-id="e3c64-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="e3c64-114">Používatelia môžu túto funkciu zapnúť alebo vypnúť v edge://settings/passwords a môžete ju nakonfigurovať v politikách [správcu hesiel](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="e3c64-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
