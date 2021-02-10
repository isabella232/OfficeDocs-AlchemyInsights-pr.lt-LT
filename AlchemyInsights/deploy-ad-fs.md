---
title: AD FS diegimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177542"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="e6e61-102">AD FS diegimas</span><span class="sxs-lookup"><span data-stu-id="e6e61-102">Deploy AD FS</span></span>

<span data-ttu-id="e6e61-103">"Active Directory" susiejimo tarnybos (AD FS) diegimas naudoja jūsų vietinę infrastruktūrą "Office 365" tarnybų vartotojams autentifikuoti.</span><span class="sxs-lookup"><span data-stu-id="e6e61-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="e6e61-104">Naudodami išorinį prisijungimo priedą, galite įgalinti vartotojus prisijungti prie "Office 365" tarnybų ir programinės įrangos kaip tarnybos (SAAS) taikomąsias programas, integruotas į "Azure Active Directory" ("Azure AD").</span><span class="sxs-lookup"><span data-stu-id="e6e61-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e6e61-105">Išorinis prisijungimas autentifikuoja vartotojus nuo vietinio "Active Directory" naudodami AD FS.</span><span class="sxs-lookup"><span data-stu-id="e6e61-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="e6e61-106">Be to, nors įmonės tinkle vartotojai nebus įpareigoti iš naujo įvesti savo slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="e6e61-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="e6e61-107">[AD FS diegimo patarėjas](https://go.microsoft.com/fwlink/?linkid=2071178) teikia išsamias instrukcijas, kaip diegti VIETINĘ AD FS infrastruktūrą, kuri autentifikuoja vartotojus, skirtus "Microsoft 365" ir "Office 365" tarnyboms.</span><span class="sxs-lookup"><span data-stu-id="e6e61-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="e6e61-108">Naudodami šį vadovą, jūsų organizacija gali peržiūrėti AD FS komponentus ir reikalavimus, įsigyti ir įdiegti SSL sertifikatus, reikalingus įdiegčiai, ir įdiegti reikiamą žiniatinklio taikomosios programos tarpinį serverį.</span><span class="sxs-lookup"><span data-stu-id="e6e61-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
