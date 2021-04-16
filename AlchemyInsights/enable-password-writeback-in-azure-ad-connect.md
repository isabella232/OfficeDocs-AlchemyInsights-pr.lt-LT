---
title: Įgalinkite slaptažodžio atgalinį įrašymą „Azure AD Connect“
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814020"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="cbd0b-102">Įgalinkite slaptažodžio atgalinį įrašymą „Azure AD Connect“</span><span class="sxs-lookup"><span data-stu-id="cbd0b-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="cbd0b-103">Jei norite įjungti savitarnos slaptažodžio nustatymo iš naujo atgalinį įrašymą, pirmiausia įgalinkite „Azure AD Connect“ atgalinio rašymo parinktį.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="cbd0b-104">Iš savo „Azure AD Connect“ serverio, atlikite toliau pateiktus veiksmus:</span><span class="sxs-lookup"><span data-stu-id="cbd0b-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="cbd0b-105">Prisijunkite prie savo „Azure AD Connect“ serverio ir įjunkite **„Azure AD Connect“** konfigūravimo vediklį.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="cbd0b-106">**Darbo pradžios** puslapyje, spustelėkite **Konfigūruoti**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="cbd0b-107">Puslapyje **Papildomos užduotys** pasirinkite **Tinkinti sinchronizavimo parinktis**, tuomet spustelėkite **Toliau**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="cbd0b-108">Puslapyje **Prisijungti prie „Azure AD“** įveskite visuotinio administratoriaus kredencialus savo „Azure“ klientui, o tuomet spustelėkite **Toliau**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="cbd0b-109">**Katalogų prijungimo** ir **Domeno/OU** filtravimo puslapiuose spustelėkite **Toliau**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="cbd0b-110">Puslapyje **Pasirenkamos funkcijos** pažymėkite langelį, esantį šalia **Slaptažodžio atgalinis įrašymas** ir spustelėkite **Toliau**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="cbd0b-111">Puslapyje **Paruošta konfigūruoti** spustelėkite **Konfigūruoti** ir palaukite, kol procesas bus baigtas.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="cbd0b-112">Kai pamatysite, kad konfigūracija baigta, spustelėkite **Išeiti**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="cbd0b-113">Įgalinę „Azure AD Connect“ slaptažodžių atgalinį įrašymą, konfigūruokite „Azure AD“ SSPR atgaliniam rašymui.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="cbd0b-114">Norėdami įgalinti atgalinį įrašymą SSPR, atlikite toliau pateiktus veiksmus:</span><span class="sxs-lookup"><span data-stu-id="cbd0b-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="cbd0b-115">Prisijunkite prie „Azure“ portalo naudodami visuotinio administratoriaus paskyrą.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="cbd0b-116">Raskite ir pasirinkite **„Azure Active Directory“**, spustelėkite **Slaptažodžio nustatymas iš naujo**, tada – **Vietinis integravimas**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="cbd0b-117">Nustatykite parinktį **Įrašyti slaptažodžius į vietinį katalogą?** į **Taip**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="cbd0b-118">Nustatykite parinktį **Leisti vartotojams atrakinti paskyras nenustačius jų slaptažodžio iš naujo?** į **Taip**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="cbd0b-119">Kai baigsite, spustelėkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-119">When ready, click **Save**.</span></span>

<span data-ttu-id="cbd0b-120">Daugiau informacijos žr. [„Azure Active Directory“ savitarnos slaptažodžio nustatymo iš naujo atgalinis įrašymas į vietinę aplinką](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="cbd0b-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="cbd0b-121">Kai administratorius iš naujo nustato vartotojo slaptažodį „Azure“ portale, jei tas vartotojas yra išorinis arba slaptažodžio maiša sinchronizuota, slaptažodis įrašomas į vietinę versiją.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="cbd0b-122">Šiai funkcijai reikalinga „Azure Premium“ licencija (P1 arba P2) ir šiuo metu ji nepalaikoma „Office“ administravimo portale.</span><span class="sxs-lookup"><span data-stu-id="cbd0b-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
