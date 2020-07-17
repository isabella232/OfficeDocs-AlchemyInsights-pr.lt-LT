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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="1d192-102">Sąlyginė prieiga su "Intune"</span><span class="sxs-lookup"><span data-stu-id="1d192-102">Conditional Access with Intune</span></span>

<span data-ttu-id="1d192-103">Norint naudoti **sąlyginę prieigą** su "Intune", reikia atlikti 3 veiksmus:</span><span class="sxs-lookup"><span data-stu-id="1d192-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="1d192-104">Sukurkite **atitikties politiką** (["Android",](https://docs.microsoft.com/intune/compliance-policy-create-android) ["iOS",](https://docs.microsoft.com/intune/compliance-policy-create-ios) ["Windows"),](https://docs.microsoft.com//intune/compliance-policy-create-windows)kad nustatytumėte parametrus, kuriuos reikia įvykdyti prieš įrenginiui laikantis.</span><span class="sxs-lookup"><span data-stu-id="1d192-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="1d192-105">Pavyzdžiui, prieš tai, kai įrenginys turi būti bent 6 skaitmenų pin, jis turi būti laikomas suderinamu.</span><span class="sxs-lookup"><span data-stu-id="1d192-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="1d192-106">Sukurkite **sąlyginės prieigos strategiją,** kuri apibrėžia, kokie ištekliai yra saugomi ir kokias sąlygas reikia įvykdyti norint pasiekti šiuos išteklius.</span><span class="sxs-lookup"><span data-stu-id="1d192-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="1d192-107">[Pavyzdžiui,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) įrenginys turi būti suderinamas prieš pasiekiant įmonės el. paštą.</span><span class="sxs-lookup"><span data-stu-id="1d192-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="1d192-108">**Užtikrinkite,** kad atitikties strategijos ir **sąlyginės prieigos strategijos** būtų taikomos norimoms vartotojų grupėms.</span><span class="sxs-lookup"><span data-stu-id="1d192-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="1d192-109">Tam gali reikėti sukurti konkrečias vartotojų grupes "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="1d192-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="1d192-110">**Naudingos nuorodos:**</span><span class="sxs-lookup"><span data-stu-id="1d192-110">**Helpful links:**</span></span>

[<span data-ttu-id="1d192-111">Įrenginio atitikties apžvalga</span><span class="sxs-lookup"><span data-stu-id="1d192-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="1d192-112">TRIKČIŲ DIAGNOSTIKA CA</span><span class="sxs-lookup"><span data-stu-id="1d192-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="1d192-113">Trikčių šalinimo strategija</span><span class="sxs-lookup"><span data-stu-id="1d192-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="1d192-114">Norint apsaugoti el. paštą ("Exchange online") nuo prieigos iš neatitinkančių įrenginių, turi būti laikomasi abiejų dokumentų:</span><span class="sxs-lookup"><span data-stu-id="1d192-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="1d192-115">Apsaugokite el. pašto prieigą iš įrenginių naudodami EAS</span><span class="sxs-lookup"><span data-stu-id="1d192-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="1d192-116">Apsaugokite el. pašto prieigą iš įrenginių naudodami modernius autentifikavimo klientus, pvz., "Outlook"</span><span class="sxs-lookup"><span data-stu-id="1d192-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)