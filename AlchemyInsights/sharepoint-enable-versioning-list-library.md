---
title: SharePoint 및 OneDrive의 버전 관리
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.custom:
- "5300025"
- "1702"
ms.openlocfilehash: 12207efc9822be6cf096fa4884a3cd244a286cbe
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800830"
---
# <a name="versioning-in-sharepoint-and-onedrive"></a><span data-ttu-id="01c24-102">SharePoint 및 OneDrive의 버전 관리</span><span class="sxs-lookup"><span data-stu-id="01c24-102">Versioning in SharePoint and OneDrive</span></span> 


<span data-ttu-id="01c24-103">SharePoint 목록 또는 라이브러리에서 버전 관리를 사용 하도록 설정 하면 목록 및 파일을 변경할 때마다 라이브러리의 항목을 저장, 추적 및 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01c24-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="01c24-104">버전 관리를 체크 아웃과 같은 다른 설정과 함께 사용 하면 사이트에 게시 되는 콘텐츠를 제어할 수 있으며 이전 버전의 항목 또는 파일을 확인 하거나 복원 해야 하는 경우 실제 가치를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="01c24-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="01c24-105">버전 관리에 대 한 자세한 내용은 다음 문서를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="01c24-105">For more information on versioning please visit the below articles.</span></span>

- [<span data-ttu-id="01c24-106">SharePoint 목록 또는 라이브러리에서 버전 관리를 사용 하는 방법</span><span class="sxs-lookup"><span data-stu-id="01c24-106">How does versioning work in a SharePoint list or library</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [<span data-ttu-id="01c24-107">목록 또는 라이브러리의 버전 관리 설정 및 구성하기</span><span class="sxs-lookup"><span data-stu-id="01c24-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f)

- [<span data-ttu-id="01c24-108">버전 기록을 보는 방법</span><span class="sxs-lookup"><span data-stu-id="01c24-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [<span data-ttu-id="01c24-109">OneDrive에서 이전 버전의 파일 복원</span><span class="sxs-lookup"><span data-stu-id="01c24-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893)

- [<span data-ttu-id="01c24-110">이전 버전의 Office 파일 보기</span><span class="sxs-lookup"><span data-stu-id="01c24-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [<span data-ttu-id="01c24-111">버전 관리 제한</span><span class="sxs-lookup"><span data-stu-id="01c24-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

>[!Note] 
><span data-ttu-id="01c24-112">Microsoft 365 고객 인 경우 새 비즈니스용 OneDrive 라이브러리를 만들 때 버전 관리가 기본적으로 설정 되며 마지막 500 버전의 문서가 자동으로 저장 됩니다.</span><span class="sxs-lookup"><span data-stu-id="01c24-112">If you are a Microsoft 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="01c24-113">이렇게 하면 중요 한 문서나 데이터가 손실 되는 것을 방지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01c24-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="01c24-114">비즈니스용 OneDrive 사이트 또는 버전 관리를 사용 하지 않는 팀 사이트에 기존 라이브러리가 있으면 언제 든 지 해당 사용자에 대해 버전 관리를 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01c24-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>


