---
title: Sąlyginė prieiga su "Intune"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931444"
---
# <a name="conditional-access-with-intune"></a>Sąlyginė prieiga su "Intune"

Norint naudoti **sąlyginę prieigą** su "Intune", reikia atlikti 3 veiksmus:

- Sukurkite **atitikties politiką** (["Android",](https://docs.microsoft.com/intune/compliance-policy-create-android) ["iOS",](https://docs.microsoft.com/intune/compliance-policy-create-ios) ["Windows"),](https://docs.microsoft.com//intune/compliance-policy-create-windows)kad nustatytumėte parametrus, kuriuos reikia įvykdyti prieš įrenginiui laikantis. Pavyzdžiui, prieš tai, kai įrenginys turi būti bent 6 skaitmenų pin, jis turi būti laikomas suderinamu.
- Sukurkite **sąlyginės prieigos strategiją,** kuri apibrėžia, kokie ištekliai yra saugomi ir kokias sąlygas reikia įvykdyti norint pasiekti šiuos išteklius.  [Pavyzdžiui,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) įrenginys turi būti suderinamas prieš pasiekiant įmonės el. paštą.
- **Užtikrinkite,** kad atitikties strategijos ir **sąlyginės prieigos strategijos** būtų taikomos norimoms vartotojų grupėms. Tam gali reikėti sukurti konkrečias vartotojų grupes "Azure Active Directory".

**Naudingos nuorodos:**

[Įrenginio atitikties apžvalga](https://docs.microsoft.com/intune/device-compliance-get-started)

[TRIKČIŲ DIAGNOSTIKA CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Trikčių šalinimo strategija](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Norint apsaugoti el. paštą ("Exchange online") nuo prieigos iš neatitinkančių įrenginių, turi būti laikomasi abiejų dokumentų:

1. [Apsaugokite el. pašto prieigą iš įrenginių naudodami EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Apsaugokite el. pašto prieigą iš įrenginių naudodami modernius autentifikavimo klientus, pvz., "Outlook"](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)