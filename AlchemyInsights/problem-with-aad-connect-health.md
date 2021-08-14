---
title: Problema su AAD Prisijungimas sveikata
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923760"
---
# <a name="problem-with-aad-connect-health"></a>Problema su AAD Prisijungimas sveikata

- Įsitikinkite, kad turite teisę atlikti operaciją. Visuotiniai administratoriai turi prieigą pagal numatytuosius parametrus. Be to, galite naudoti [vaidmenimis pagrįstą prieigos valdiklį norėdami](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) perduoti registracijos teises bendraautoriui.
- Įsitikinkite, kad reikiami galiniai punktai įgalinti, o ne blokuojami dėl užkardos. Daugiau informacijos žr. [reikalavimai](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija gali nepavykti dėl siunčiamo ryšio, kai tinklo lygmuo tikrina SSL.
- Įsitikinkite, kad patvirtinote "Azure AD Prisijungimas Health" pranešimų parametrus. Peržiūrėkite savo parametrą. Šis [vadovas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) gali padėti suprasti, kaip konfigūruoti "Azure AD" pranešimų parametrus Prisijungimas sveikatos pranešimus.
- Norėdami sužinoti daugiau apie AAD Prisijungimas sveikatos sinchronizavimo ataskaitą ir kaip ją atsisiųsti, žr. [Objektų lygio sinchronizavimo ataskaita](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Norėdami šalinti "AAD Prisijungimas Health" įspėjimų triktis, vykdykite ["AAD Prisijungimas Health data freshness"](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) įspėjimų ir dažnai užduodamų klausimų trikčių šalinimo vadovą, žr. ["Common AAD Prisijungimas Health installation questions".](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
