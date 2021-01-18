---
title: Konfigūruoti LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885571"
---
# <a name="configure-ldap"></a>Konfigūruoti LDAP

Norėdami konfigūruoti LDAP, atlikite šiuos veiksmus:

1. Patikrinkite savo domeno sveikatą "Azure" [portale](https://aka.ms/aadds-health).
1. Įsitikinkite, kad yra galiojanti "Azure AD" prenumerata ir įgalintas "Azure AD" domenų tarnybos.
1. Norint įgalinti apsaugotą LDAP sertifikatą reikia gauti patikimos viešosios sertifikavimo institucijos arba vartotojo pasirašomą sertifikatą.
1. Įsitikinkite, kad sertifikatas atitinka reikiamas [gaires](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Netinkamas sertifikatas**
1. Norėdami atnaujinti sertifikatą, atlikite veiksmus, kad sukurtumėte naują sertifikatą, ir iš naujo nusiųsti: [Konfigūruokite LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Norėdami išspręsti žinomą problemą, susijusią su saugiais LDAP įspėjimais "Azure Active Directory" domenų tarnybose, skaitykite [LDAP įspėjimų](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)sprendimo būdas.
