---
title: 126 OWA nepavyksta rasti klaidos gaunant pašto dėžutę?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426670"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="af32f-102">Gaunate pašto dėžutę, kurios nepavyko rasti internetinėje "Outlook"?</span><span class="sxs-lookup"><span data-stu-id="af32f-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="af32f-103">Jei naudojate internetinę "Outlook" ir  nepavyksta rasti klaidos pašto dėžutės, paskyra, kurią naudojote prisijungdami prie internetinės "Outlook", neturi "Exchange Online" licencijos, todėl jokia pašto dėžutė nėra susieta su paskyra.</span><span class="sxs-lookup"><span data-stu-id="af32f-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="af32f-104">Administratorius gali priskirti jūsų paskyrai licenciją, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="af32f-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="af32f-105">Atidarykite ["Microsoft 365"](https://portal.office.com/adminportal/home#/homepage)  administravimo centrą  ir eikite į Aktyvūs vartotojai dalyje Vartotojai ir pasirinkite vartotoją, kuris mato klaidą.</span><span class="sxs-lookup"><span data-stu-id="af32f-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="af32f-106">Atidaromame vartotojo puslapyje eikite į sekciją **Licencijos** ir taikomosios programos, pasirinkite atitinkamą **vietos reikšmę** ir priskirkite licenciją, kurioje yra "Exchange Online" (išplėskite licenciją, kad pamatytumėte jos informaciją).</span><span class="sxs-lookup"><span data-stu-id="af32f-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="af32f-107">Kai baigsite, spustelėkite Įrašyti **keitimus**.</span><span class="sxs-lookup"><span data-stu-id="af32f-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="af32f-108">Kai kuriais atvejais, jei licencija jau priskirta vartotojo paskyrai, pašalinus ir persignuojant licenciją galima išspręsti problemą ir tinkamai ją parengti sistemoje:</span><span class="sxs-lookup"><span data-stu-id="af32f-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="af32f-109">Patikrinkite, ar jūsų M365 "Exchange Online" (ir kitos, jei turite) prenumeratos yra dabartinės ir pastaruoju metu jų galiojimas nesibaigė.</span><span class="sxs-lookup"><span data-stu-id="af32f-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="af32f-110">Kai įsitikinsite, kad jūsų prenumeratos galiojimas nepasibaigė ir vartotojo paskyrai priskirta galiojanti licencija, gali užtrukti iki 24 valandų, kol licencija bus susaista, todėl gali tekti palaukti, kol problema bus išspręsta.</span><span class="sxs-lookup"><span data-stu-id="af32f-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="af32f-111">Daugiau informacijos [žr. Licencijų priskyrimas ir valdymas](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span><span class="sxs-lookup"><span data-stu-id="af32f-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>