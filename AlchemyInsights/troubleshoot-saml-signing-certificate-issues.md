---
title: "\"SAML\" pasirašymas sertifikato problemų šalinimas"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693426"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="5a0d7-102">"SAML" pasirašymas sertifikato problemų šalinimas</span><span class="sxs-lookup"><span data-stu-id="5a0d7-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="5a0d7-103">Norėdami išspręsti problemą, atlikite šiuos rekomenduojamus veiksmus:</span><span class="sxs-lookup"><span data-stu-id="5a0d7-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="5a0d7-104">Kai įtraukiate įmonės programą, kuri palaiko SSO, "Azure" sukurs sertifikatą, vadinamą [SAML pasirašytu sertifikatu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="5a0d7-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="5a0d7-105">Šio sertifikato galiojimo laikas yra 3 metai.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="5a0d7-106">Norėdami pakeisti sertifikato galiojimo pabaigos datą, peržiūrėkite [savo susiejimo sertifikato galiojimo pabaigos datos tinkinimą ir pervyniokite jį į naują sertifikatą](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="5a0d7-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="5a0d7-107">"Azure" naudos šį sertifikatą, kad būtų galima prisijungti prie taikomosios programos pareikalautą SAML žetonų ir nusiųsti jį į sėkmingą SSO programą.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="5a0d7-108">Kad tai užbaigtumėte, atsisiųskite sertifikatą iš "Azure" portalo ir nusiųskite jį į taikomosios programos pardavėją, kad užbaigtumėte SSO procesą.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="5a0d7-109">Užbaigus šį procesą, programa pasitikės šį sertifikatą ir visi šio sertifikato pasirašyti SAML žetonai bus priimti naudojant taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="5a0d7-110">Jei šio sertifikato galiojimo laikas baigėsi, sukurkite naują sertifikatą, atnaujinkite jį taikomosios programos tiekėju ir suaktyvinkite jį "Azure" šone.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="5a0d7-111">Daugiau informacijos ieškokite [sertifikato atnaujinimas, kurio galiojimas greitai baigsis](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="5a0d7-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="5a0d7-112">Jei sertifikato galiojimo laikas baigėsi, vartotojas nebus užblokuotas.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="5a0d7-113">[Įtraukite el. pašto adresą, kad pranešimai](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) būtų gauti iki esamo sertifikato galiojimo pabaigos.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="5a0d7-114">4 veiksmas yra pasirinktinis.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="5a0d7-115">Pakeiskite programos SAML sertifikato pasirašymas parinktis ir sertifikato pasirašymas algoritmas.</span><span class="sxs-lookup"><span data-stu-id="5a0d7-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="5a0d7-116">Daugiau informacijos rasite [sertifikato pasirašymas parinkčių keitimas ir pasirašančiojo algoritmas](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="5a0d7-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

