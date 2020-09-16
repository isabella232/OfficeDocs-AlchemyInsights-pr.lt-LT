---
title: Failas atidaromas tik skaityti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745599"
---
# <a name="file-open-read-only"></a><span data-ttu-id="a5605-102">Failas atidaromas tik skaityti</span><span class="sxs-lookup"><span data-stu-id="a5605-102">File open read-only</span></span>

<span data-ttu-id="a5605-103">Galite pastebėti, kad atidarant failus, jie atidaromi kaip skirti tik skaityti.</span><span class="sxs-lookup"><span data-stu-id="a5605-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="a5605-104">Kai kuriais atvejais tai yra papildoma sauga, pvz., kai atidarote failus iš interneto, ir kitą laiką, taip gali būti dėl parametrų, kuriuos galima keisti.</span><span class="sxs-lookup"><span data-stu-id="a5605-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="a5605-105">Toliau pateikiami keli scenarijai, kai failas atidaromas tik skaityti ir keli veiksmai, kuriuos galite atlikti Norėdami pakeisti.</span><span class="sxs-lookup"><span data-stu-id="a5605-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="a5605-106">**Mano antivirusinė sukelia jiems atidaryti tik skaityti**</span><span class="sxs-lookup"><span data-stu-id="a5605-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="a5605-107">Kai kurios antivirusinės programos gali apsaugoti jus nuo potencialiai nesaugių failų atidarydami jas tik skaityti.</span><span class="sxs-lookup"><span data-stu-id="a5605-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="a5605-108">Norint sužinoti, kaip pakoreguoti šiuos parametrus, gali reikėti susisiekti su savo antivirusinės programos teikėju.</span><span class="sxs-lookup"><span data-stu-id="a5605-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="a5605-109">Pvz., BitDefender turi turinio įtraukti taikomosios programos išimtis: [kaip įtraukti taikomosios programos arba proceso išskyrimų "BitDefender" valdymo centre](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="a5605-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="a5605-110">**Ar failų ypatybės nustatytos tik skaityti?**</span><span class="sxs-lookup"><span data-stu-id="a5605-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="a5605-111">Galite patikrinti failo ypatybes, dešiniuoju pelės mygtuku spustelėdami failą ir pasirinkdami ypatybės.</span><span class="sxs-lookup"><span data-stu-id="a5605-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="a5605-112">Jei pažymėtas atributas tik skaityti, galite jį nuimti ir spustelėti Gerai.</span><span class="sxs-lookup"><span data-stu-id="a5605-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="a5605-113">**Turinys yra apsaugotame rodinyje**</span><span class="sxs-lookup"><span data-stu-id="a5605-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="a5605-114">Failuose iš interneto ir kitų potencialiai nesaugių vietų gali būti virusų, kirminų arba kitų kenkėjiškų programų, galinčių pakenkti jūsų kompiuteriui.</span><span class="sxs-lookup"><span data-stu-id="a5605-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="a5605-115">Tai taip pat paprastai taikoma naudojant elektroninio pašto priedus arba atsisiųstus failus.</span><span class="sxs-lookup"><span data-stu-id="a5605-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="a5605-116">Siekiant apsaugoti kompiuterį, failai iš potencialiai nesaugių vietų atidaromi apsaugotame rodinyje.</span><span class="sxs-lookup"><span data-stu-id="a5605-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="a5605-117">Naudodami apsaugotą rodinį, galite skaityti failą ir matyti jo turinį, mažindami riziką.</span><span class="sxs-lookup"><span data-stu-id="a5605-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="a5605-118">Daugiau informacijos apie apsaugotą rodinį ir kaip pakeisti parametrus rasite šiame straipsnyje: [kas yra apsaugotas rodinys?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="a5605-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="a5605-119">**Ar "OneDrive" U3/4imta?**</span><span class="sxs-lookup"><span data-stu-id="a5605-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="a5605-120">Jei failas saugomas "OneDrive" ir jūsų "OneDrive" saugyklos vieta yra visa, negalėsite įrašyti dokumento, kol nebūsite po jūsų skirtu tarpu.</span><span class="sxs-lookup"><span data-stu-id="a5605-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="a5605-121">Galite patikrinti savo laisvą vietą "OneDrive", spustelėdami "OneDrive" piktogramą informacinių pranešimų centre ir pasirinkdami valdyti saugyklą arba galite eiti į, [https://onedrive.live.com](https://onedrive.live.com) prisijungti ir įsidėmėti, kiek naudojamos vietos yra ekrano apatiniame kairiajame kampe.</span><span class="sxs-lookup"><span data-stu-id="a5605-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="a5605-122">**Ar "Office" suaktyvinta?**</span><span class="sxs-lookup"><span data-stu-id="a5605-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="a5605-123">Jei "Office" nesuaktyvintas arba jūsų produktų paketo galiojimo laikas baigėsi, galite būti tik skaitymo sumažinto funkcionalumo režimu.</span><span class="sxs-lookup"><span data-stu-id="a5605-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="a5605-124">Informacijos, kaip aktyvinti "Office", ieškokite: [nelicencijuoto produkto ir aktyvinimo klaidos "Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)".</span><span class="sxs-lookup"><span data-stu-id="a5605-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="a5605-125">**Jei visa kita nepavyksta...**</span><span class="sxs-lookup"><span data-stu-id="a5605-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="a5605-126">Pabandykite iš naujo paleisti kompiuterį</span><span class="sxs-lookup"><span data-stu-id="a5605-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="a5605-127">"Office" naujinimų diegimas</span><span class="sxs-lookup"><span data-stu-id="a5605-127">Install Office updates</span></span>
    
- <span data-ttu-id="a5605-128">"Office" taisymo internete atlikimas</span><span class="sxs-lookup"><span data-stu-id="a5605-128">Perform an Online repair of Office</span></span>
    

