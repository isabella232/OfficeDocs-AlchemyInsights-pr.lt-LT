---
title: Išorinių vartotojų įtraukimas į paskirstymo grupę
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737881"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="030e0-102">Išorinių vartotojų įtraukimas į paskirstymo grupę</span><span class="sxs-lookup"><span data-stu-id="030e0-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="030e0-103">Išorinio kontakto įtraukimas į paskirstymo grupę (DG) yra dviejų etapų procesas:</span><span class="sxs-lookup"><span data-stu-id="030e0-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="030e0-104">Pašto kontakto kūrimas Išoriniam vartotojui:</span><span class="sxs-lookup"><span data-stu-id="030e0-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="030e0-105">Administravimo centre eikite į puslapį **vartotojų** > [Kontaktai](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="030e0-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="030e0-106">Pasirinkite **įtraukti kontaktą**.</span><span class="sxs-lookup"><span data-stu-id="030e0-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="030e0-107">Įveskite kontakto informaciją ir pasirinkite **įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="030e0-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="030e0-108">Pridėti pašto kontaktą savo GD:</span><span class="sxs-lookup"><span data-stu-id="030e0-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="030e0-109">Administravimo centre eikite į **grupių** > [grupių](https://admin.microsoft.com/adminportal/home#/groups) puslapį.</span><span class="sxs-lookup"><span data-stu-id="030e0-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="030e0-110">Suraskite GD, į kurį norite įtraukti išorinį vartotoją, ir pasirinkite jį, kad atidarytumėte redagavimo dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="030e0-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="030e0-111">Skirtuke **nariai** pasirinkite **Peržiūrėti viską ir valdykite narius**.</span><span class="sxs-lookup"><span data-stu-id="030e0-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="030e0-112">Pasirinkite **Įtraukti narių**.</span><span class="sxs-lookup"><span data-stu-id="030e0-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="030e0-113">Pasirinkite pašto kontaktą, kurį sukūrėte atlikdami ankstesnį veiksmą, ir pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="030e0-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="030e0-114">Jei atlikę šiuos veiksmus Išoriniai vartotojai negalės siųsti el. laiškų generaliniam direktoratui arba iš jo negaunate el. laiškų, gali būti, kad GD pažymėtas tik leisti el. laiškus iš vidinių vartotojų.</span><span class="sxs-lookup"><span data-stu-id="030e0-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="030e0-115">Galite patikrinti šią konfigūraciją ir ją sutvarkyti taip, kaip nurodyta [toliau.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="030e0-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="030e0-116">**Pastaba:** Šios instrukcijos netaikomos, jei jūsų grupės tipas yra "Office 365 Group" vietoj "paskirstymo grupė".</span><span class="sxs-lookup"><span data-stu-id="030e0-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="030e0-117">Tokiu atveju išorinį vartotoją galite įtraukti tiesiai į grupę iš "Outlook".</span><span class="sxs-lookup"><span data-stu-id="030e0-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="030e0-118">Išsami informacija apie Office 365 grupių svečiai, taip pat instrukcijas, kaip pridėti išorinių Svečių, galima rasti [šiame straipsnyje](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="030e0-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  