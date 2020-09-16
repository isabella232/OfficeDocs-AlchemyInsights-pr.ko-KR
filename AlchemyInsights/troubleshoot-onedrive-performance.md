---
title: OneDrive 성능 문제 해결
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757891"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="90003-102">OneDrive 성능 문제 해결</span><span class="sxs-lookup"><span data-stu-id="90003-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="90003-103">예상 동기화 속도 보다 느리거나 OneDrive와 유사한 성능 문제가 발생 하는 경우:</span><span class="sxs-lookup"><span data-stu-id="90003-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="90003-104">[서비스 상태 대시보드](https://portal.office.com/adminportal/home?ref=/servicehealth)를 사용할 때 알려진 문제가 없는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="90003-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="90003-105">[필요할 때 파일을 사용 하도록 설정](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) 하 여 모든 파일을 다운로드 하거나 장치에서 저장소 공간을 사용 하지 않고 OneDrive에서 모든 사용자에 게 액세스할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="90003-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="90003-106">네트워크 계획 및 성능에 대 한 모범 [사례를 검토](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) 합니다.</span><span class="sxs-lookup"><span data-stu-id="90003-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="90003-107">[업로드 및 다운로드 속도를 최대화](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)합니다 (특히 장치를 처음으로 동기화 하는 경우).</span><span class="sxs-lookup"><span data-stu-id="90003-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="90003-108">라이브러리를 10만 개 보다 많은 항목을 동기화 하는 경우 OneDrive 동기화가 오랜 시간 동안 중지 된 것 처럼 보이거나 상태에 xMB의 처리 0KB 표시 됩니다. "</span><span class="sxs-lookup"><span data-stu-id="90003-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="90003-109">[10만 개 보다 많은 파일을 동기화 하는 방법에 대해 자세히 알아보고](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) [OneDrive의 지원 되는 30만 파일 제한을](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)확인 하세요.</span><span class="sxs-lookup"><span data-stu-id="90003-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="90003-110">사용자가 사용 한도를 초과 하는 경우 SharePoint Online은 짧은 기간 동안 해당 사용자 계정에서 더 이상 요청을 제한 합니다.</span><span class="sxs-lookup"><span data-stu-id="90003-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="90003-111">스로틀가 적용 되는 동안에는 모든 사용자 작업이 제한 됩니다.</span><span class="sxs-lookup"><span data-stu-id="90003-111">All user actions are throttled while the throttle is in effect.</span></span>
