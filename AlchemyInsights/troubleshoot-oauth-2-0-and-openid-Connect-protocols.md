---
title: Riešenie problémov s OAuth 2,0 a OpenID Connect Protocols
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
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037699"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Riešenie problémov s OAuth 2,0 a OpenID Connect Protocols

Ak chcete vyriešiť problémy s OAuth 2,0 a OpenID Connect, vykonajte tieto Odporúčané kroky:

Pozrite si nasledujúce články, ktoré súvisia s konfiguráciou a riešením problémov s OAuth 2,0 a OpenID Connect Protocols:

- [Microsoft Identity Platform a OAuth 2,0 autorizačný kód flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – v tomto článku sa popisuje, ako v aplikácii použiť ľubovoľný jazyk priamo voči **toku kódu grantu (PKCE)** .
- [Microsoft Identity Platform a tok poverení klienta OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – v tomto článku sa popisuje, ako program priamo v porovnaní s **tokom poverení klienta** v aplikácii.
- [Microsoft Identity Platform a OAuth 2,0 zdrojov poverenia vlastníka hesla](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – v tomto článku sa popisuje, ako sa program priamo v porovnaní s **ROPC tokom** v aplikácii.
    - Platforma Microsoft Identity podporuje iba ROPC pre nájomníkov služby Azure AD a nie pre osobné kontá. Znamená to, že je nutné použiť koncový bod pre nájomníka **( https://login.microsoftonline.com/{TenantId_or_Name})** alebo koncový bod **organizácie** .
    - Osobné kontá, ktoré sú pozvaní na nájomníka služby Azure AD, nemôžu používať ROPC.
    - Kontá, ktoré nemajú heslá, sa nemôžu prihlásiť cez ROPC. Pre tento scenár odporúčame použiť iný tok pre aplikáciu namiesto toho.
    - Ak používatelia potrebujú na prihlásenie do aplikácie používať [viacnásobné overovanie (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) , budú zablokovaní.
    - ROPC nie je podporovaná v scenároch [hybridnej identity federácie](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (napríklad Azure AD a ADFS používané na overenie lokálnych kont). Ak sú používatelia na celú stránku presmerovaní na lokálneho poskytovateľa identity, Azure AD nedokáže otestovať meno používateľa a heslo voči danému poskytovateľovi identity. Pri ROPC sa však podporuje [overovanie prenesenia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) .
    - Výnimka z scenára hybridnej identity federácie by bola nasledujúca: politika zisťovania domovskej oblasti s **AllowCloudPasswordValidation** nastavená na **hodnotu True** umožní ROPC toku pracovať pre externých používateľov, keď je lokálne heslo synchronizované s cloudom. Ďalšie informácie nájdete v téme [povolenie priameho ROPC overovania externých používateľov pre staršie aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Platforma Microsoft identity a OAuth 2,0 v mene toku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – v tomto článku sa popisuje, ako v aplikácii priamo naprogramovať v rámci **toku (OBO)** .
- [Microsoft Identity Platform a OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – v tomto článku sa dozviete, ako implementovať protokol OpenID Connect nezávislý od jazyka, a popisuje spôsob odosielania a prijímania správ http bez použitia akýchkoľvek knižníc s otvorenými zdrojmi Microsoft.

**Prístupové tokeny**

[Tokeny prístupu k platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Zistite, ako môže vaše rozhranie API overiť a použiť nároky v accessovom tokene. Celá dokumentácia v tomto článku s výnimkou prípadov, keď je uvedené, sa vzťahuje len na tokeny vydané pre rozhrania API, ktoré ste zaregistrovali. Nevzťahuje sa na tokeny vydané pre rozhrania API vo vlastníctve spoločnosti Microsoft a nie je možné použiť tieto tokeny na overenie, akým spôsobom bude platforma Microsoft Identity vydávať tokeny pre vytvorené API.

**Konfigurácia aplikácie**

[Obmedzenia a obmedzenia presmerovania URI (URL adresy odpovedí)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Zistite, ako nakonfigurovať identifikátor URI presmerovania (URL adresy). Identifikátor URI presmerovania alebo adresa URL odpovede, je miesto, kde server autorizácie odošle používateľovi po úspešnom schválení aplikácie a udelení autorizačného kódu alebo accessového tokenu. Server autorizácie odošle kód alebo token do identifikátora URI presmerovania. je dôležité, aby ste si zaregistrovali správne umiestnenie ako súčasť procesu registrácie aplikácie.

**Poskytovanie aplikácií**

[Kurz: vytvorenie a plánovanie poskytovania koncového bodu scim](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – v tomto článku sa popisuje postup pri zostavovaní koncového bodu scim a integrácii pomocou poskytovania služby AAD.


