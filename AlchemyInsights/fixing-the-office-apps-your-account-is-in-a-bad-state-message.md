---
title: Oprava aplikácií balíka Office váš účet je v zlom stave správy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969781"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="6785b-102">Oprava aplikácie balíka Office "váš účet je v zlom stave" chyba</span><span class="sxs-lookup"><span data-stu-id="6785b-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="6785b-103">Ak chcete opraviť túto chybu, vyskúšajte nasledujúce možnosti na postihnutý počítač:</span><span class="sxs-lookup"><span data-stu-id="6785b-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="6785b-104">Otvorte aplikáciu balíka Office, vyberte položku**konto** >  **súboru** > **odhlásiť zo všetkých účtov**.</span><span class="sxs-lookup"><span data-stu-id="6785b-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="6785b-105">Prihláste sa znova pomocou používateľského konta s platnou licenciou.</span><span class="sxs-lookup"><span data-stu-id="6785b-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="6785b-106">Podrobné informácie nájdete v téme [kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="6785b-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="6785b-107">[Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="6785b-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="6785b-108">**Poznámka:** Cesty databázy Registry pre balík Office 2016 sa zmenili na 16,0.</span><span class="sxs-lookup"><span data-stu-id="6785b-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6785b-109">Napríklad \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="6785b-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="6785b-110">Na postihnutý počítač, nastavte EnableADAL = 0 pomocou nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="6785b-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="6785b-111">Kliknite pravým tlačidlom myši na tlačidlo Windows a vyberte **Spustiť**.</span><span class="sxs-lookup"><span data-stu-id="6785b-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="6785b-112">Do poľa **Otvoriť** zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="6785b-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="6785b-113">Ak sa zobrazí výzva na povolenie editora databázy Registry, vyberte možnosť **Yes (Áno** ), čím vykonáte zmeny v zariadení.</span><span class="sxs-lookup"><span data-stu-id="6785b-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="6785b-114">V editore databázy Registry pridajte hodnotu DWORD EnableADAL s nastavením 0 podľa HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="6785b-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="6785b-115">Ak sa vyskytne chyba pri pripájaní k Office 365 pomocou Office 2013, [Povoliť moderné overovanie](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) pre klienta Office.</span><span class="sxs-lookup"><span data-stu-id="6785b-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="6785b-116">Ďalšie informácie nájdete v téme [Riešenie problémov s aplikáciami, ktoré nie sú prehľadávačom, ktoré sa nedajú prihlásiť do balíka Office 365, Azure alebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="6785b-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

