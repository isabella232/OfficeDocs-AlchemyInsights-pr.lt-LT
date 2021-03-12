---
title: Saugos centre nepavyko rasti prenumeratos
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713959"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="139de-102">Saugos centre nepavyko rasti prenumeratos</span><span class="sxs-lookup"><span data-stu-id="139de-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="139de-103">Jei prie "Microsoft Defender" saugos centro gaunate pranešimą "nėra prenumeratų", tai reiškia, kad "Azure Active Directory" (AAD), naudojama vartotojui prisijungti prie portalo, nėra "Microsoft Defender ATP" licencijos.</span><span class="sxs-lookup"><span data-stu-id="139de-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="139de-104">"Windows E5" ir "Office E5" licencijos yra atskiros licencijos.</span><span class="sxs-lookup"><span data-stu-id="139de-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="139de-105">Atidarykite palaikymo atvejį, jei licencija buvo įsigyta, bet neparengta šiam AAD egzemplioriui.</span><span class="sxs-lookup"><span data-stu-id="139de-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="139de-106">Turite:</span><span class="sxs-lookup"><span data-stu-id="139de-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="139de-107">Galima licencijos parengimo problema.</span><span class="sxs-lookup"><span data-stu-id="139de-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="139de-108">Netyčia parengėte licenciją kitam "Microsoft AAD" nei ta, kurią naudojote autentifikavimui.</span><span class="sxs-lookup"><span data-stu-id="139de-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>