---
title: Problemos, susijusios su besiūlių SSO integravimu su mano vietinėje programėlėmis
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868717"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="0447b-102">Problemos, susijusios su besiūlių SSO integravimu su mano vietinėje programėlėmis</span><span class="sxs-lookup"><span data-stu-id="0447b-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="0447b-103">Norėdami šalinti triktis, susijusias su sklandžiais SSO integravimu su vietinėse taikomosiose programose, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="0447b-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="0447b-104">**Rekomenduojami veiksmai**</span><span class="sxs-lookup"><span data-stu-id="0447b-104">**Recommended steps**</span></span>

1. <span data-ttu-id="0447b-105">Norėdami sukonfigūruoti **vietinę taikomąją** programą, skirtą **vienkartiniam autentifikacija naudojant taikomosios programos tarpinį serverį**, peržiūrėkite [bendrosios autentifikacijos slaptažodį naudojant taikomosios programos tarpinį serverį](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="0447b-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="0447b-106">**Taikomųjų programų tarpinio serverio problemų trikčių diagnostika**: rekomenduojame pradėti peržiūrėti trikčių šalinimo srautą, [derinti taikomosios programos tarpinio serverio jungties problemas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), kad nustatytumėte, ar taikomosios programos tarpinio serverio jungtys tinkamai sukonfigūruotos.</span><span class="sxs-lookup"><span data-stu-id="0447b-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="0447b-107">Jei vis dar kyla problemų jungiantis prie taikomosios programos, vadovaukitės trikčių šalinimo veiksmais [derinimo taikomosios programos tarpinio serverio taikomosios programos problemoms spręsti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="0447b-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="0447b-108">" [CORS" problemas galite identifikuoti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) naudodami šiuos naršyklės derinimo įrankius:</span><span class="sxs-lookup"><span data-stu-id="0447b-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="0447b-109">Paleisk naršyklę ir naršykite į žiniatinklio programą.</span><span class="sxs-lookup"><span data-stu-id="0447b-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="0447b-110">Paspauskite **F12** , kad iškviestumėte derinimo konsolę.</span><span class="sxs-lookup"><span data-stu-id="0447b-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="0447b-111">Pabandykite atkurti operaciją ir peržiūrėkite konsolės pranešimą.</span><span class="sxs-lookup"><span data-stu-id="0447b-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="0447b-112">CORS pažeidimas sukuria konsolės klaidą apie kilmę.</span><span class="sxs-lookup"><span data-stu-id="0447b-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="0447b-113">Kai kurios "CORS" problemos neišsprendžiamos, pvz., kai jūsų programa nukreipia į "login.microsoftonline.com" ir "Access" atpažinimo ženklo galiojimo laikas baigsis.</span><span class="sxs-lookup"><span data-stu-id="0447b-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="0447b-114">Tada nepavyksta.</span><span class="sxs-lookup"><span data-stu-id="0447b-114">The CORS call then fails.</span></span> <span data-ttu-id="0447b-115">Šio scenarijaus sprendimo būdas – pratęsti "Access" atpažinimo ženklo galiojimo laiką, kad jis nesibaigtų vartotojo seanso metu.</span><span class="sxs-lookup"><span data-stu-id="0447b-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="0447b-116">Daugiau informacijos apie tai, kaip tai padaryti, rasite [konfigūruotina atpažinimo ženklų naudojimo "Microsoft" tapatybės platformoje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)informacija.</span><span class="sxs-lookup"><span data-stu-id="0447b-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="0447b-117">**Rekomenduojami dokumentai**</span><span class="sxs-lookup"><span data-stu-id="0447b-117">**Recommended documents**</span></span>

- [<span data-ttu-id="0447b-118">Kaip sukonfigūruoti bendrąją autentifikacija taikomosios programos tarpinio serverio taikomajai programai</span><span class="sxs-lookup"><span data-stu-id="0447b-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="0447b-119">SAML vienkartinė autentifikacija vietinėms programoms naudojant taikomosios programos tarpinį serverį</span><span class="sxs-lookup"><span data-stu-id="0447b-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="0447b-120">"Azure Active Directory" taikomųjų programų tarpinio serverio problemų supratimas ir sprendimas</span><span class="sxs-lookup"><span data-stu-id="0447b-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="0447b-121">"Kerberos" ribojami taikomųjų programų tarpinio serverio perdavimo konfigūracijų trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="0447b-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)