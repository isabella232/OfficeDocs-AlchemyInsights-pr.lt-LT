---
title: "\"Microsoft Intune\" saugos bazinių linijų naudojimas norint sukonfigūruoti \"Windows 10\" įrenginius"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573537"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="3153c-102">"Microsoft Intune" saugos bazinių linijų naudojimas norint sukonfigūruoti "Windows 10" įrenginius</span><span class="sxs-lookup"><span data-stu-id="3153c-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="3153c-103">"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius.</span><span class="sxs-lookup"><span data-stu-id="3153c-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="3153c-104">Saugos bazinės linijos yra "Windows" parametrų iš anksto sukonfigūruotos grupės, naudojamos, kad būtų taikoma žinoma grupės parametrai ir numatytosios reikšmės, rekomenduojamos atitinkamų saugos komandų.</span><span class="sxs-lookup"><span data-stu-id="3153c-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="3153c-105">Sukūrę saugos bazinės linijos profilį "Intune", sukuriate šabloną, sudarytą iš kelių įrenginių konfigūracijos profilių.</span><span class="sxs-lookup"><span data-stu-id="3153c-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="3153c-106">Kai saugos bazinės linijos diegiamos vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, kurie veikia "Windows 10" arba naujesnę versiją.</span><span class="sxs-lookup"><span data-stu-id="3153c-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="3153c-107">Pvz., MDM saugos bazinės linijos Automatinis (1) įjungia "BitLocker", skirtą keičiamiesiems diskams (2), reikia slaptažodžio atrakinimo, ir (3) išjungia bazinį autentifikavimą.</span><span class="sxs-lookup"><span data-stu-id="3153c-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="3153c-108">Kai numatytoji reikšmė neveikia jūsų aplinkoje, tinkinkite bazinę liniją, kad pritaikytumėte norimus parametrus.</span><span class="sxs-lookup"><span data-stu-id="3153c-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="3153c-109">Saugumo bazinės linijos taip pat padeda sukurti saugią "Microsoft 365" darbo eigą.</span><span class="sxs-lookup"><span data-stu-id="3153c-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="3153c-110">Toliau pateikiami keli pranašumai:</span><span class="sxs-lookup"><span data-stu-id="3153c-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="3153c-111">Saugos bazinė linija aprėpia geriausią praktiką ir parametrų, kurie turi įtakos saugai, rekomendacijas.</span><span class="sxs-lookup"><span data-stu-id="3153c-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="3153c-112">Kadangi "Intune" partneriai su "Windows" saugos komanda, kuri sukuria grupės strategijų bazinių linijų, šios rekomendacijos pagrįstos tvirta rekomendacija ir didelė patirtimi.</span><span class="sxs-lookup"><span data-stu-id="3153c-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="3153c-113">Jei esate naujokas "Intune" ir nežinote, nuo ko pradėti, tada saugos bazinės linijos padės jums greitai sukurti ir įdiegti saugų profilį.</span><span class="sxs-lookup"><span data-stu-id="3153c-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="3153c-114">Jei šiuo metu naudojate grupės strategiją, perėjimas prie Intune valdymo tikslais yra daug lengviau su saugos bazinių linijų, nes jie yra integruoti į Intune ir apima pažangiausius valdymo pajėgumus.</span><span class="sxs-lookup"><span data-stu-id="3153c-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="3153c-115">Norėdami sužinoti daugiau, žiūrėkite ["Windows" saugos bazinės linijos](https://go.microsoft.com/fwlink/?linkid=2141503) ir [mobiliųjų įrenginių valdymas](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="3153c-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>