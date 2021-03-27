---
title: Išplėstinės autentifikavimo sąvokos, taikomos "Microsoft Edge"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398593"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="d2c44-102">Išplėstinės autentifikavimo sąvokos, taikomos "Microsoft Edge"</span><span class="sxs-lookup"><span data-stu-id="d2c44-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="d2c44-103">Toliau nurodytos išplėstinės autentifikavimo sąvokos, taikomos "Microsoft Edge":</span><span class="sxs-lookup"><span data-stu-id="d2c44-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="d2c44-104">**Aktyvus autentifikavimas**</span><span class="sxs-lookup"><span data-stu-id="d2c44-104">**Proactive Authentication**</span></span>

<span data-ttu-id="d2c44-105">Kai įgalinsite ["ProactiveAuthEnabled"](https://go.microsoft.com/fwlink/?linkid=2134621) strategiją, "Microsoft Edge" bandys aktyviai autentifikuoti prisijungusius vartotojus per "Microsoft" tarnybas.</span><span class="sxs-lookup"><span data-stu-id="d2c44-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="d2c44-106">Reguliariais intervalais ji naudos internetinę tarnybą, kad patikrins, ar yra atnaujinta deklaracija, kurioje yra konfigūracija, reglamentuojanti aktyvią autentifikavimą.</span><span class="sxs-lookup"><span data-stu-id="d2c44-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="d2c44-107">Pranašumai: aktyvus autentifikavimas įgalina autentifikavimą pagrindinėse tarnybose, pvz., "Office" naujo skirtuko puslapyje.</span><span class="sxs-lookup"><span data-stu-id="d2c44-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="d2c44-108">Be to, jei "Bing" naudojama kaip ieškos modulis, aktyvus autentifikavimas pagerina adreso juostos našumą ir padeda generuoti ieškos rezultatus, pritaikytus jūsų verslo poreikiams.</span><span class="sxs-lookup"><span data-stu-id="d2c44-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="d2c44-109">**"Windows Hello CredUI", skirta "NTLM" autentifikavimui**</span><span class="sxs-lookup"><span data-stu-id="d2c44-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="d2c44-110">Jei bendroji autentifikacija (SSO) negalima, kai žiniatinklio svetainė bando prisijungti prie vartotojo naudodama NTLM arba "Negotiate" mechanizmą, ši funkcija leis vartotojui bendrinti OS kredencialus su svetaine ir patenkinti autentifikavimo iššūkius naudojant "Windows Hello Cred" vartotojo sąsają.</span><span class="sxs-lookup"><span data-stu-id="d2c44-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="d2c44-111">Šis prisijungimo srautas bus rodomas tik "Windows 10" ir tik vartotojams, kurie negaus SSO NTLM arba "Negotiate" iššūkio metu.</span><span class="sxs-lookup"><span data-stu-id="d2c44-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="d2c44-112">**Įrašytų slaptažodžių naudojimas norint prisijungti automatiškai**</span><span class="sxs-lookup"><span data-stu-id="d2c44-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="d2c44-113">Vartotojai, įrašę slaptažodžius "Microsoft Edge", gali įgalinti automatinį prisijungimą prie svetainių, kuriose įrašė kredencialus.</span><span class="sxs-lookup"><span data-stu-id="d2c44-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="d2c44-114">Vartotojai gali įjungti arba išjungti šią funkciją "edge://settings/passwords ir galite konfigūruoti ją slaptažodžių [tvarkytuvo strategijose.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="d2c44-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
