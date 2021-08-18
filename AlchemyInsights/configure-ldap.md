---
title: LDAP konfigūravimas
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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090420"
---
# <a name="configure-ldap"></a>LDAP konfigūravimas

Norėdami konfigūruoti LDAP, atlikite šiuos veiksmus:

1. Patikrinkite savo domeno sveikatą ["Azure" portale.](https://aka.ms/aadds-health)
1. Įsitikinkite, kad yra galiojanti "Azure AD" prenumerata ir įgalinta "Azure AD" domenų tarnyba.
1. Sertifikatas, būtinas saugiam LDAP įgalinti, turi būti gautas iš patikimos viešosios sertifikavimo institucijos arba būti pasirašytas.
1. Įsitikinkite, kad sertifikatas yra toks, kaip [reikalaujama.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Netinkamas sertifikatas**
1. Norėdami atnaujinti sertifikatą, atlikite veiksmus, kad sukurtumėte naują sertifikatą ir iš naujo įkeltumėte: [Konfigūruokite LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Norėdami išspręsti žinomas "Azure Active directory" domenų tarnybų saugos LDAP įspėjimų problemas, žr. [LDAP įspėjimų sprendimas](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
