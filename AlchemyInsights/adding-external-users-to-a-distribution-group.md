---
title: Išorinių vartotojų įtraukimas į platinimo grupę
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663521"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="c748a-102">Išorinių vartotojų įtraukimas į platinimo grupę</span><span class="sxs-lookup"><span data-stu-id="c748a-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="c748a-103">Išorinio kontakto įtraukimas į platinimo grupę (DG) yra dviejų etapų procesas:</span><span class="sxs-lookup"><span data-stu-id="c748a-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="c748a-104">Išorinio vartotojo pašto kontakto kūrimas:</span><span class="sxs-lookup"><span data-stu-id="c748a-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="c748a-105">Administravimo centre eikite į puslapį **vartotojų**  >  [Kontaktai](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="c748a-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="c748a-106">Pasirinkite **įtraukti kontaktą**.</span><span class="sxs-lookup"><span data-stu-id="c748a-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="c748a-107">Įveskite kontakto informaciją ir pasirinkite **įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="c748a-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="c748a-108">Įtraukite pašto kontaktą į savo GD:</span><span class="sxs-lookup"><span data-stu-id="c748a-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="c748a-109">Administravimo centre eikite į puslapį **grupių**  >  [grupės](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="c748a-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="c748a-110">Raskite generalinį direktoratą, į kurį norite įtraukti išorinį vartotoją, ir pasirinkite jį, kad atidarytumėte dialogo langą redagavimas.</span><span class="sxs-lookup"><span data-stu-id="c748a-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="c748a-111">Skirtuke **nariai** pasirinkite **Peržiūrėti visus ir valdykite narius**.</span><span class="sxs-lookup"><span data-stu-id="c748a-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="c748a-112">Pasirinkite **įtraukti narius**.</span><span class="sxs-lookup"><span data-stu-id="c748a-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="c748a-113">Pasirinkite pašto kontaktą, kurį sukūrėte atlikdami ankstesnį veiksmą, tada pasirinkite **įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="c748a-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="c748a-114">Jei atlikus šiuos veiksmus, Išoriniai vartotojai negali siųsti el. laiškų generaliniam direktoratui arba negauna iš jo gautų laiškų, gali būti, kad GD yra pažymėtas tik leisti laiškus iš vidinių vartotojų.</span><span class="sxs-lookup"><span data-stu-id="c748a-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="c748a-115">Galite patikrinti šį konfigūravimą ir ją pataisyti vykdydami nurodymus [čia](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="c748a-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="c748a-116">**Pastaba:** Šios instrukcijos netaikomos, jei jūsų grupės tipas yra "Microsoft 365 Group", o ne "Distribution Group".</span><span class="sxs-lookup"><span data-stu-id="c748a-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="c748a-117">Jei tai yra atvejis, galite tiesiogiai įtraukti išorinį vartotoją į grupę iš "Outlook".</span><span class="sxs-lookup"><span data-stu-id="c748a-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="c748a-118">Išsamios informacijos apie "Microsoft" 365 grupių svečių ir išorinių Svečių įtraukimo instrukcijas rasite [šiame straipsnyje](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="c748a-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  