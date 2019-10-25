---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682216"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>FIX el. pašto pristatymo problemos klaidos kodas 5.7.23

Patikrinkite savo domeno SPF DNS įrašą viešai prieinamoje SPF arba DNS įrašų tikrintuve žiniatinklyje.

Patikrinkite, ar siunčiamojo laiško nebuvo nustatyta kaip šlamštas Office 365 ir nukreipiami per [didelis rizikos pristatymo telkinys](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Didelės rizikos pristatymo telkinio pranešimai nepraeis SPF patikros, todėl paskirties el. pašto organizacijos nepriims.

Jei problema kartojasi, jums gali tekti susisiekti su pašto serverio, į kurį bandote siųsti el. laišką, administratoriumi. Užsirašykite išsamią išorinę klaidą peradresavimo pranešime.  Office 365 parama gali nepavykti toliau.