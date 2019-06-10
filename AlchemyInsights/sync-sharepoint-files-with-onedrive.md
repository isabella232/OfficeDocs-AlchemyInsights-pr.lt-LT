---
title: „SharePoint“ failų sinchronizavimas naudojant naująjį „OneDrive“ sinchronizavimo klientą
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757826"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="0d909-102">„SharePoint“ failų sinchronizavimas naudojant naująjį „OneDrive“ sinchronizavimo klientą</span><span class="sxs-lookup"><span data-stu-id="0d909-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="0d909-103">Komanda Atidaryti naudojant „Explorer“ atidaro vietinį „Windows Explorer“ egzempliorių, kuriame rodoma aplanko struktūra serveryje, kuriame yra „SharePoint“ svetainė.</span><span class="sxs-lookup"><span data-stu-id="0d909-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="0d909-104">Atsižvelgiant į tai, rekomenduojame [sinchronizuoti „SharePoint“ failus su naujuoju „OneDrive“ sinchronizavimo klientu](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, kuris teikia [failus pagal pareikalavimą](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), nes jis suteikia vietinę prieigą prie jūsų failų ir siūlo geriausią našumą.</span><span class="sxs-lookup"><span data-stu-id="0d909-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="0d909-105">Jei pasirinkote naudoti „Explorer“ rodinį, o ne naująjį sinchronizavimo klientą, būtinai atlikite toliau pateiktuose straipsniuose nurodytus veiksmus ir naudokitės ten aprašytais geriausios praktikos pavyzdžiais.</span><span class="sxs-lookup"><span data-stu-id="0d909-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="0d909-106">Kaip naudoti komandą Atidaryti naudojant „Explorer“, norint išspręsti triktis „SharePoint Online“</span><span class="sxs-lookup"><span data-stu-id="0d909-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="0d909-107">Bibliotekos failų kopijavimas arba perkėlimas naudojant parinktį Atidaryti naudojant „Explorer“</span><span class="sxs-lookup"><span data-stu-id="0d909-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="0d909-108">Pastaba: mygtukas Atidaryti naudojant „Explorer“ nerodomas naujojoje bibliotekos sąsajoje.</span><span class="sxs-lookup"><span data-stu-id="0d909-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="0d909-109">Viršutiniame dešiniajame kampe spustelėkite išplečiamąjį sąrašą Rodinys (išplečiamojo sąrašo pavadinimas keičiasi, atsižvelgiant į dabartinį rodinį), tada failų naršyklėje spustelėkite Rodinys. </span><span class="sxs-lookup"><span data-stu-id="0d909-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="0d909-110">„SharePoint“ komanda Atidaryti naudojant „Explorer“ naudoja „ActiveX“ valdiklius, todėl ji palaikoma tik „Internet Explorer“ 10 arba 11 versijoje.</span><span class="sxs-lookup"><span data-stu-id="0d909-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="0d909-111">Komanda Atidaryti naudojant „Explorer“ neveikia sistemoje „Windows“ su „Microsoft Edge“, „Google Chrome“ ir „Mozilla Firefox“ arba „Mac“ platformoje.</span><span class="sxs-lookup"><span data-stu-id="0d909-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="0d909-112">Dėl šios priežasties „Explorer“ rodinio parinktis gali būti papilkinta.</span><span class="sxs-lookup"><span data-stu-id="0d909-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="0d909-113">[Kodėl „SharePoint“ juostelės mygtukai nepasiekiami arba papilkinti](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="0d909-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

