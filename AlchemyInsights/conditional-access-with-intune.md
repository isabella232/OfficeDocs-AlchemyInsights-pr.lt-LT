---
title: Sąlyginė prieiga su Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807667"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="2017a-102">Sąlyginė prieiga su Intune</span><span class="sxs-lookup"><span data-stu-id="2017a-102">Conditional Access with Intune</span></span>

<span data-ttu-id="2017a-103">Naudojant  **sąlyginę prieigą**  su Intune reikia 3 veiksmų:</span><span class="sxs-lookup"><span data-stu-id="2017a-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="2017a-104">Sukurkite  **atitikties strategiją**  (["Android](https://docs.microsoft.com/intune/compliance-policy-create-android)", "  [ios](https://docs.microsoft.com/intune/compliance-policy-create-ios)",  ["Windows"](https://docs.microsoft.com//intune/compliance-policy-create-windows)), kad nustatytumėte parametrus, kuriuos reikia atitikti prieš tai, kai prietaisas laikomas atitinkančiu reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="2017a-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="2017a-105">Pvz., įrenginyje turi būti bent 6 skaitmenų PIN, kad jis būtų laikomas atitinkančiu reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="2017a-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="2017a-106">Sukurkite **sąlyginės prieigos strategiją**  , kuri apibrėžia, kokie ištekliai yra saugomi, ir kokiomis sąlygomis reikia pasiekti šiuos išteklius.</span><span class="sxs-lookup"><span data-stu-id="2017a-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="2017a-107">[Pavyzdžiui,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  įrenginys turi būti suderinamas prieš jungiantis prie įmonės elektroninio pašto.</span><span class="sxs-lookup"><span data-stu-id="2017a-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="2017a-108">Užtikrinkite, kad **atitikties strategijos**  ir  **sąlyginės prieigos strategijos**  būtų nukreiptos į pageidaujamas vartotojų grupes.</span><span class="sxs-lookup"><span data-stu-id="2017a-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="2017a-109">Tam gali reikėti sukurti tam tikras vartotojų grupes "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="2017a-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="2017a-110">**Naudingi saitai:**</span><span class="sxs-lookup"><span data-stu-id="2017a-110">**Helpful links:**</span></span>

[<span data-ttu-id="2017a-111">Įrenginio atitikties apžvalga</span><span class="sxs-lookup"><span data-stu-id="2017a-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="2017a-112">Trikčių diagnostika CA</span><span class="sxs-lookup"><span data-stu-id="2017a-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="2017a-113">Trikčių šalinimo strategija</span><span class="sxs-lookup"><span data-stu-id="2017a-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="2017a-114">Norint apsaugoti el. paštą ("Exchange Online") iš "Access" neatitinkančius įrenginius, būtina laikytis abiejų dokumentų:</span><span class="sxs-lookup"><span data-stu-id="2017a-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="2017a-115">El. pašto prieigos apsauga iš įrenginių, naudojančių EAS</span><span class="sxs-lookup"><span data-stu-id="2017a-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="2017a-116">Apsaugoti pašto prieigą iš įrenginių, naudojančių šiuolaikinius autentifikavimo klientus, pvz., "Outlook"</span><span class="sxs-lookup"><span data-stu-id="2017a-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)