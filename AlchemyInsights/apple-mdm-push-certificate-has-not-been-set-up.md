---
title: Apple MDM Push sertifikatas nenustatytas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439379"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push sertifikatas nenustatytas

"Apple MDM Push" sertifikatas (dar vadinamas "Apple Push Notification Service" (APNS) sertifikatu) nebuvo sukonfigūruotas jūsų prenumeratai. Be sukonfigūruotos "Apple MDM Push" sertifikato negalite registruotis ir valdyti "iOS" ir "Mac OS" įrenginių. Įtraukę sertifikatą į "Intune", vartotojai gali įdiegti programą Įmonės portalas, kad užregistruotų savo "iOS" įrenginius.

1. Pasirinkite **"Sutinku".** suteikti "Microsoft" leidimą siųsti duomenis "Apple".

2. Pasirinkite **Atsisiųsti savo ĮSA** Intune sertifikato pasirašymo užklausą, reikalingą sukurti Apple MDM push sertifikatą. Failas naudojamas norint prašyti patikimo ryšio sertifikato iš "Apple Push" sertifikatų portalo.

3. Pasirinkite **Sukurti savo MDM push sertifikatą,** kad pereitumėte į "Apple Push" sertifikatų portalą. Prisijunkite naudodami savo įmonės "Apple ID", tada pasirinkite **Sukurti sertifikatą**. Pasirinkite **Pasirinkti failą**, raskite sertifikato pasirašymo užklausos failą, tada pasirinkite **Nusiųsti**. Puslapyje Patvirtinimas pasirinkite **Atsisiųsti,** kad atsisiųstumėte sertifikato (.pem) failą ir įrašytumėte failą vietoje.
 
**Pastaba:** sertifikatas susietas su "Apple ID", naudojamu jam sukurti. Geriausia būtų naudoti įmonės "Apple ID" valdymo užduotims atlikti ir įsitikinti, kad pašto dėžutę stebi daugiau nei vienas asmuo arba naudodami siuntimo sąrašą. Niekada nenaudokite asmeninio "Apple ID". Naudokite tą patį "Apple ID", kad atnaujintumėte "Apple Push" sertifikatą kas 12 mėnesių.
 
4. Įveskite "Apple ID", naudojamą "Apple MDM" "push" sertifikatui sukurti. Įrašykite šį ID kaip priminimą, kai reikia atnaujinti sertifikatą.

5. Eikite į sertifikato (.pem) failą, pasirinkite **Atidaryti**, tada pasirinkite **Nusiųsti**. Su push sertifikatą, Intune gali registruotis ir valdyti Apple įrenginius.