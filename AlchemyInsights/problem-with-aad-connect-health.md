---
title: "\"AAD Connect Health\" problema"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482071"
---
# <a name="problem-with-aad-connect-health"></a>"AAD Connect Health" problema

- Įsitikinkite, kad turite teisę atlikti veiksmą. Visuotiniai administratoriai turi prieigą pagal numatytuosius numatytuosius. Be to, galite naudoti [vaidmenimis pagrįstą prieigos valdymą](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , kad galėtumėte perduoti registravimo teisę bendraautoriui.
- Užtikrinkite, kad būtini galiniai punktai yra įgalinti ir Neblokuojami dėl užkardos. Išsamesnės informacijos ieškokite [reikalavimai](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija gali nepavykti dėl išeinančio ryšio su tinklo lygiu atliekama SSL patikra.
- Įsitikinkite, kad patikrinote "Azure AD Connect Health" pranešimų parametrus. Peržiūrėkite savo parametrą. Šis [vadovas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) gali padėti suprasti, kaip konfigūruoti pranešimų parametrus "Azure AD Connect Health" pranešimuose.
- Norėdami sužinoti daugiau apie "AAD Connect Health" sinchronizavimo ataskaitą ir kaip ją atsisiųsti, žiūrėkite [objekto lygio sinchronizavimo ataskaita](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Norėdami pašalinti "AAD Connect Health" įspėjimus, vadovaukitės [trikčių diagnostikos vadovu, kad galėtumėte susisiekti su sveikatos duomenų šviežumo įspėjimais](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ir dažniausiai užduodamais klausimais, skaitykite [bendrosios "AAD Connect Health" klausimai](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
