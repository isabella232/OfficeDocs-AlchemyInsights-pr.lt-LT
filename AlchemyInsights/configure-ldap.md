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
# <a name="configure-ldap"></a><span data-ttu-id="99ef6-102">Konfigūruoti LDAP</span><span class="sxs-lookup"><span data-stu-id="99ef6-102">Configure LDAP</span></span>

<span data-ttu-id="99ef6-103">Norėdami konfigūruoti LDAP, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="99ef6-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="99ef6-104">Patikrinkite savo domeno sveikatą "Azure" [portale](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="99ef6-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="99ef6-105">Įsitikinkite, kad yra galiojanti "Azure AD" prenumerata ir įgalintas "Azure AD" domenų tarnybos.</span><span class="sxs-lookup"><span data-stu-id="99ef6-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="99ef6-106">Norint įgalinti apsaugotą LDAP sertifikatą reikia gauti patikimos viešosios sertifikavimo institucijos arba vartotojo pasirašomą sertifikatą.</span><span class="sxs-lookup"><span data-stu-id="99ef6-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="99ef6-107">Įsitikinkite, kad sertifikatas atitinka reikiamas [gaires](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="99ef6-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="99ef6-108">**Netinkamas sertifikatas**</span><span class="sxs-lookup"><span data-stu-id="99ef6-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="99ef6-109">Norėdami atnaujinti sertifikatą, atlikite veiksmus, kad sukurtumėte naują sertifikatą, ir iš naujo nusiųsti: [Konfigūruokite LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="99ef6-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="99ef6-110">Norėdami išspręsti žinomą problemą, susijusią su saugiais LDAP įspėjimais "Azure Active Directory" domenų tarnybose, skaitykite [LDAP įspėjimų](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)sprendimo būdas.</span><span class="sxs-lookup"><span data-stu-id="99ef6-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
