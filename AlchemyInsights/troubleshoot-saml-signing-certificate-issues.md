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
# <a name="troubleshoot-saml-signing-certificate-issues"></a>"SAML" pasirašymas sertifikato problemų šalinimas

Norėdami išspręsti problemą, atlikite šiuos rekomenduojamus veiksmus:

1. Kai įtraukiate įmonės programą, kuri palaiko SSO, "Azure" sukurs sertifikatą, vadinamą [SAML pasirašytu sertifikatu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Šio sertifikato galiojimo laikas yra 3 metai. Norėdami pakeisti sertifikato galiojimo pabaigos datą, peržiūrėkite [savo susiejimo sertifikato galiojimo pabaigos datos tinkinimą ir pervyniokite jį į naują sertifikatą](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. "Azure" naudos šį sertifikatą, kad būtų galima prisijungti prie taikomosios programos pareikalautą SAML žetonų ir nusiųsti jį į sėkmingą SSO programą. Kad tai užbaigtumėte, atsisiųskite sertifikatą iš "Azure" portalo ir nusiųskite jį į taikomosios programos pardavėją, kad užbaigtumėte SSO procesą.

Užbaigus šį procesą, programa pasitikės šį sertifikatą ir visi šio sertifikato pasirašyti SAML žetonai bus priimti naudojant taikomąją programą.

3. Jei šio sertifikato galiojimo laikas baigėsi, sukurkite naują sertifikatą, atnaujinkite jį taikomosios programos tiekėju ir suaktyvinkite jį "Azure" šone. Daugiau informacijos ieškokite [sertifikato atnaujinimas, kurio galiojimas greitai baigsis](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Jei sertifikato galiojimo laikas baigėsi, vartotojas nebus užblokuotas.

4. [Įtraukite el. pašto adresą, kad pranešimai](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) būtų gauti iki esamo sertifikato galiojimo pabaigos.

> [!NOTE]
> 4 veiksmas yra pasirinktinis.

5. Pakeiskite programos SAML sertifikato pasirašymas parinktis ir sertifikato pasirašymas algoritmas. Daugiau informacijos rasite [sertifikato pasirašymas parinkčių keitimas ir pasirašančiojo algoritmas](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

