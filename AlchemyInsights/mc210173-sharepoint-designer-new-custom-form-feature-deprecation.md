---
title: MC210173 - SharePoint Designer의 새 사용자 지정 양식 기능 사용 중단
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: a53b8885a877cb688cfb42bb4f9108cb2cef2418
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743886"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="2567e-102">MC210173 - SharePoint Designer의 새 사용자 지정 양식 기능 사용 중단</span><span class="sxs-lookup"><span data-stu-id="2567e-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="2567e-103">Sharepoint Online 내에서 [사용자 지정 양식 만들기](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)를 위한 SharePoint Designer 기능에 영향을 미치는 문제를 확인했습니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="2567e-104">신중히 검토한 후, 이 문제에 대해 알려진 수정 방법이 없으며 2020년 4월 25일 토요일 오전 3시(UTC)부터 사용자 지정 양식 만들기 기능의 사용 중단을 결정했습니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="2567e-105">이 변경 사항은 SharePoint Online Designer에서 이전에 만든 양식을 편집하는 기능이나 다른 기존 기능에는 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="2567e-106">이 변경 사항이 적용되면 새 양식을 만들 때 "목록 변경 사항을 서버에 저장할 수 없습니다."라는 오류 메시지가 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="2567e-107">이전에 활용한 SharePoint Designer로 사용자 지정 양식을 만들려는 사용자는 [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form)를 대신 활용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="2567e-108">PowerApps는 사용자가 SharePoint Online 최신 환경에서, 브라우저 창에서 바로 SharePoint 목록과 문서 라이브러리에 대한 사용자 지정 양식을 만들거나 편집하는 작업을 수행할 수 있게 해주는 쉽고 강력한 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="2567e-109">PowerApps는 기존 코딩 지식이나 InfoPath 등의 추가적인 앱 다운로드도 요구하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="2567e-110">**참고**: SharePoint Online 클래식 사용자는 PowerApps에 액세스하고 활용하기 위해 일시적으로 최신 환경으로 전환해야 합니다. 하지만 SharePoint Online 클래식 환경 사용자는 PowerApps에서 만든 모든 사용자 지정 양식에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2567e-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
