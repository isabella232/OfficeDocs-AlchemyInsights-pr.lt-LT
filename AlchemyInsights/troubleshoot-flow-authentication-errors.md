---
title: Srauto autentifikavimo klaidų šalinimas
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690575"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="4466e-102">Srauto autentifikavimo klaidų šalinimas</span><span class="sxs-lookup"><span data-stu-id="4466e-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="4466e-103">Daugeliu atvejų nepavyksta dėl autentifikavimo klaidos.</span><span class="sxs-lookup"><span data-stu-id="4466e-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="4466e-104">Jei yra tokio tipo klaida, klaidos pranešime yra "neteisėtas" arba "401" arba "403" klaidos kodas.</span><span class="sxs-lookup"><span data-stu-id="4466e-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="4466e-105">Paprastai autentifikavimo klaidą galite išspręsti atnaujindami jungtį:</span><span class="sxs-lookup"><span data-stu-id="4466e-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="4466e-106">Žiniatinklio portalo viršuje spustelėkite arba bakstelėkite krumpliaračio piktogramą, kad atidarytumėte meniu parametrai, tada spustelėkite arba bakstelėkite **ryšiai**.</span><span class="sxs-lookup"><span data-stu-id="4466e-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="4466e-107">Slinkite į jungtį, kurioje matėte neleistiną klaidos pranešimą.</span><span class="sxs-lookup"><span data-stu-id="4466e-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="4466e-108">Prie ryšio spustelėkite arba bakstelėkite saitą **patvirtinti slaptažodį** , esantį pranešime apie ryšį, kuris nėra autentifikuotas.</span><span class="sxs-lookup"><span data-stu-id="4466e-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="4466e-109">Patvirtinkite savo kredencialus vykdydami rodomas instrukcijas, grįžkite į savo srauto apdorojimo triktis, tada spustelėkite arba bakstelėkite **iš naujo pateikti**.</span><span class="sxs-lookup"><span data-stu-id="4466e-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="4466e-110">Jei turite daugiau pagalbos, žiūrėkite [srauto trikčių diagnostika](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="4466e-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

