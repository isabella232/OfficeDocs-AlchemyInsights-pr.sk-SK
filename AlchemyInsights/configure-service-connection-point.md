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
# <a name="configure-service-connection-point-scp"></a>Konfigurovanie bodu pripojenia služby (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Dôvod**: nie je možné prečítať objekt SCP a získať informácie o nájomníkovi služby Azure AD
- **Riešenie**: Prečítajte si časť [Konfigurácia bodu pripojenia služby](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Akčný plán**

- Skontrolujte, či zariadenie prijalo objekt GPO na kontrolované overenie.
- Presvedčte sa, že objekt GPO vytvoril kľúče databázy Registry.
- Uistite sa, že máte 2 kľúče vytvorené pomocou IDENTIFIKÁTORa adresára a domény onmicrosoft.

**Konfigurácia nastavenia databázy Registry na strane klienta pre SCP**

Použite nasledujúci príklad na vytvorenie objektu skupinovej politiky (GPO) na nasadenie nastavenia databázy Registry, ktoré konfiguruje položku SCP v databáze Registry svojich zariadení.

1. Otvorte konzolu na správu skupinovej politiky a vytvorte nový objekt GPO v doméne.
     - Poskytnite svoj novovytvorený objekt GPO názov (napríklad ClientSideSCP)

2. Upravte objekt GPO a vyhľadajte nasledujúcu cestu: **Konfigurácia počítača > predvoľby > nastavenie systému Windows > Registry**.

3. Kliknite pravým tlačidlom myši na **databázu Registry** a vyberte položku **Nová položka databázy Registry >**.

4. Na karte **Všeobecné** nakonfigurujte nasledovné:
  
- **Akcia**: Aktualizácia
    
- **Úľ**: HKEY_LOCAL_MACHINE
    
- **Cesta ku kľúču**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Názov hodnoty**: nájomníka
    
- **Typ hodnoty**: REG_SZ
    
- **Údaje o hodnote**: identifikátor GUID alebo adresár vašej inštancie služby Azure AD (Táto hodnota sa nachádza na **portáli Azure Portal > azure Active Directory > vlastnosti > ID adresára**)
 
- Kliknite na tlačidlo **OK**.
 
5. Kliknite pravým tlačidlom myši na **databázu Registry** a vyberte položku **Nová položka databázy Registry >**.

6. Na karte **Všeobecné** nakonfigurujte nasledovné:
  
- **Akcia**: Aktualizácia
    
- **Úľ**: HKEY_LOCAL_MACHINE
    
- **Cesta ku kľúču**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Názov hodnoty**: TenantName
    
- **Typ hodnoty**: REG_SZ
    
- **Údaje o hodnote**: názov overeného názvu domény, ak používate externé prostredie, akým je napríklad AD FS. Váš overený názov domény alebo názov domény onmicrosoft.com (napríklad contoso. onmicrosoft). com, ak používate spravované prostredie

- Kliknite na tlačidlo **OK**.

7. Zatvorenie editora pre novovytvorený objekt GPO.

8. Prepojiť novovytvorený objekt GPO s požadovanou OU, ktorá obsahuje počítače pripojené k doméne, ktoré patria do kontrolovaného zavádzacieho súboru.

Ďalšie informácie nájdete v téme [riadené overovanie hybridného spojenia Azure AD – Azure AD | Dokumenty spoločnosti Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) a  [Riešenie problémov hybridných zariadení spojených so službou Azure Active Directory | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









