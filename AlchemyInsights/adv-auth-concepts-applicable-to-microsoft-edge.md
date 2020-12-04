---
title: Išplėstinės autentifikavimo koncepcijos, taikomos "Microsoft Edge"
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573524"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="414fd-102">Išplėstinės autentifikavimo koncepcijos, taikomos "Microsoft Edge"</span><span class="sxs-lookup"><span data-stu-id="414fd-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="414fd-103">Toliau pateiktos išplėstinės autentifikavimo koncepcijos, kurios taikomos "Microsoft Edge":</span><span class="sxs-lookup"><span data-stu-id="414fd-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="414fd-104">**Iniciatyvi autentifikacija**</span><span class="sxs-lookup"><span data-stu-id="414fd-104">**Proactive Authentication**</span></span>

<span data-ttu-id="414fd-105">Kai įgalinate strategiją [Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) , "Microsoft Edge" bandys aktyviai autentifikuoti prisijungusiems vartotojams per "Microsoft" tarnybas.</span><span class="sxs-lookup"><span data-stu-id="414fd-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="414fd-106">Reguliariais intervalais ji naudos internetinę paslaugą, kad tikrintų, ar yra atnaujinta deklaracija, kurioje yra aktyvi konfigūracija.</span><span class="sxs-lookup"><span data-stu-id="414fd-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="414fd-107">Pranašumai: aktyvus autentifikavimas įgalina autentifikavimo pagrindines tarnybas, pvz., "Office" naujo skirtuko puslapį.</span><span class="sxs-lookup"><span data-stu-id="414fd-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="414fd-108">Be to, jei kaip ieškos modulį naudojamas "Bing", aktyvusis autentifikavimas pagerina adreso juostos veikimą ir padeda sukurti suasmenintus ieškos rezultatus pagal jūsų įmonės poreikius.</span><span class="sxs-lookup"><span data-stu-id="414fd-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="414fd-109">**"Windows Hello" Creipt NTLM autentifikavimui**</span><span class="sxs-lookup"><span data-stu-id="414fd-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="414fd-110">Jei Bendroji autentifikacija (SSO) neprieinama, kai žiniatinklio svetainė bando prisijungti vartotojui per NTLM arba Negotiate mechanizmą, ši funkcija leis vartotojui bendrinti OS kredencialus su svetaine ir patenkinti autentifikavimo iššūkį naudojant "Windows Hello" CRED UI.</span><span class="sxs-lookup"><span data-stu-id="414fd-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="414fd-111">Šis prisijungimo srautas bus rodomas tik sistemoje "Windows 10" ir tik tiems vartotojams, kurie negauna SSO per NTLM arba Negotiate iššūkį.</span><span class="sxs-lookup"><span data-stu-id="414fd-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="414fd-112">**Naudokite įrašytus slaptažodžius, kad prisijungtumėte automatiškai**</span><span class="sxs-lookup"><span data-stu-id="414fd-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="414fd-113">Vartotojai, kurie įrašo slaptažodžius "Microsoft Edge", gali įgalinti automatinį prisiregistravimo žiniatinklio svetaines, kuriose yra įrašytų kredencialų.</span><span class="sxs-lookup"><span data-stu-id="414fd-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="414fd-114">Vartotojai gali įjungti arba išjungti šią funkciją "edge://settings/passwords", o jūs galite ją sukonfigūruoti [slaptažodžių tvarkytuvo](https://go.microsoft.com/fwlink/?linkid=2134622) politikoje.</span><span class="sxs-lookup"><span data-stu-id="414fd-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
