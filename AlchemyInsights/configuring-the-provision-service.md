---
title: Nuostatų paslaugos konfigūravimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482872"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="e28b4-102">Nuostatų paslaugos konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="e28b4-102">Configuring the Provision service</span></span>

<span data-ttu-id="e28b4-103">Jei reikia automatizuoto vartotojo parengimo darbui, "Azure AD" reikia galiojančių kredencialų, leidžiančių prisijungti prie darbo dienos žiniatinklio tarnybų API.</span><span class="sxs-lookup"><span data-stu-id="e28b4-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="e28b4-104">Be to, "Test Connection" mygtukas darbo dieną, skirtas skelbimų vartotojo parengimo programėlei, taip pat patikrina, ar jis gali prisijungti prie "Azure AD Connect" parengimo agento, susieto su skelbimo domenu.</span><span class="sxs-lookup"><span data-stu-id="e28b4-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="e28b4-105">Jei "Azure" portale įrašant kredencialus grąžinama klaida, atlikite toliau nurodytus rekomenduojamus veiksmus:</span><span class="sxs-lookup"><span data-stu-id="e28b4-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="e28b4-106">Įsitikinkite, kad esate sukonfigūravę darbo dienos integravimo sistemos vartotojo abonementą, kaip nurodyta skyriuje mokomųjų [vartotojų integravimo sistemos vartotojo darbo dienos konfigūravimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="e28b4-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="e28b4-107">Įsitikinkite, kad "Azure AD Connect" parengimo agento tarnyba veikia ir veikia jūsų vietiniame "Windows Server", naudodami tarnybų valdymo konsolę.</span><span class="sxs-lookup"><span data-stu-id="e28b4-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="e28b4-108">Taip pat galite patikrinti agento būseną "Azure" portale spustelėdami mygtuką Peržiūrėti vietinius agentus.</span><span class="sxs-lookup"><span data-stu-id="e28b4-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="e28b4-109">Įsitikinkite, kad įvedate lauko "WORKDAY username" reikšmę naudodami formatą username@workday – nuomotojo vardas.</span><span class="sxs-lookup"><span data-stu-id="e28b4-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="e28b4-110">Jei darbo dienos – nuomotojo vardo nėra, nepavyksta autentifikuoti darbo dieną.</span><span class="sxs-lookup"><span data-stu-id="e28b4-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="e28b4-111">Jei konfigūruojate integraciją su "WORKDAY" diegimo nuomotoju, Įsiminkite jūsų darbo dienos nuomotojo suplanuotus prastovos valandas.</span><span class="sxs-lookup"><span data-stu-id="e28b4-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="e28b4-112">Darbo diena suplanavo laiką savo įgyvendinimo nuomotojams per savaitgalius (paprastai nuo penktadienio vakaro iki šeštadienio ryto) ir ryšio triktys šio prastovų lange yra žinoma problema, kurią automatiškai išsprendžia, kai tik įgyvendinimo nuomotojai grįžta internete.</span><span class="sxs-lookup"><span data-stu-id="e28b4-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="e28b4-113">Retais atvejais taip pat galite matyti šią klaidą, jei integravimo sistemos vartotojo slaptažodis buvo pakeistas dėl nuomotojo atnaujinimo arba paskyra yra užrakintoje arba pasibaigutoje būsenoje.</span><span class="sxs-lookup"><span data-stu-id="e28b4-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="e28b4-114">Patikrinkite integravimo sistemos vartotojo būseną su savo darbo dienos administratoriumi.</span><span class="sxs-lookup"><span data-stu-id="e28b4-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="e28b4-115">Išsamesnės informacijos apie darbo dienos konfigūravimą automatiniam parengimas ieškokite straipsnyje [Susipažinkite: darbo dienos konfigūravimas automatiniam vartotojų parengimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="e28b4-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
