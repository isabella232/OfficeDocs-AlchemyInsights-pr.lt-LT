---
title: "\"Microsoft Intune\" saugos bazinių linijų naudojimas norint sukonfigūruoti \"Windows 10\" įrenginius"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696388"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="938cd-102">"Microsoft Intune" saugos bazinių linijų naudojimas konfigūruojant "Windows 10" įrenginius</span><span class="sxs-lookup"><span data-stu-id="938cd-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="938cd-103">"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius.</span><span class="sxs-lookup"><span data-stu-id="938cd-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="938cd-104">Saugos bazinės linijos yra "Windows" parametrų iš anksto sukonfigūruotos grupės, naudojamos, kad būtų taikoma žinoma grupės parametrai ir numatytosios reikšmės, rekomenduojamos atitinkamų saugos komandų.</span><span class="sxs-lookup"><span data-stu-id="938cd-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="938cd-105">Sukūrę saugos bazinės linijos profilį "Intune", sukuriate šabloną, sudarytą iš kelių įrenginių konfigūracijos profilių.</span><span class="sxs-lookup"><span data-stu-id="938cd-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="938cd-106">Kai saugos bazinės linijos diegiamos vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, kurie veikia "Windows 10" arba naujesnėse versijose.</span><span class="sxs-lookup"><span data-stu-id="938cd-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="938cd-107">Pvz., "Microsoft" mobiliųjų įrenginių valdymo (MDM) saugos bazinės linijos Automatinis (1) įgalina "BitLocker", skirtą keičiamiesiems diskams (2), reikalauja slaptažodžio atrakinimo įrenginio ir (3) išjungia bazinį autentifikavimą.</span><span class="sxs-lookup"><span data-stu-id="938cd-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="938cd-108">Kai numatytoji reikšmė neveikia jūsų aplinkoje, galite tinkinti bazinę liniją, kad pritaikytumėte norimus parametrus.</span><span class="sxs-lookup"><span data-stu-id="938cd-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="938cd-109">Saugumo bazinės linijos taip pat padeda sukurti saugią "Microsoft 365" darbo eigą.</span><span class="sxs-lookup"><span data-stu-id="938cd-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="938cd-110">Toliau pateikiami kai kurie šios funkcijos pranašumai:</span><span class="sxs-lookup"><span data-stu-id="938cd-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="938cd-111">Saugos bazinė linija aprėpia geriausią praktiką ir parametrų, kurie turi įtakos saugai, rekomendacijas.</span><span class="sxs-lookup"><span data-stu-id="938cd-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="938cd-112">Kadangi "Intune" partneriai su "Windows" saugos komanda, kuri sukuria grupės strategijų bazinių linijų, šios rekomendacijos pagrįstos tvirta rekomendacija ir didelė patirtimi.</span><span class="sxs-lookup"><span data-stu-id="938cd-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="938cd-113">Jei esate naujokas "Intune" ir nežinote, nuo ko pradėti, tada saugos bazinės linijos padės jums greitai sukurti ir įdiegti saugų profilį.</span><span class="sxs-lookup"><span data-stu-id="938cd-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="938cd-114">Jei šiuo metu naudojate grupės strategiją, perėjimas prie Intune valdymo tikslais yra daug lengviau su saugos bazinių linijų, nes šios saugos bazinės linijos yra įtaisytos į Intune ir apima pažangiausius valdymo pajėgumus.</span><span class="sxs-lookup"><span data-stu-id="938cd-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="938cd-115">Daugiau informacijos ieškokite ["Windows" saugos bazinės linijos](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) ir [mobiliųjų įrenginių valdymas](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="938cd-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>