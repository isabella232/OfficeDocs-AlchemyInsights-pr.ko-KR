---
title: SharePoint, OneDrive 및 Microsoft Teams에 대해 Office 365용 Defender
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543583"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="c7be8-102">SharePoint, OneDrive 및 Microsoft Teams에 대해 Office 365용 Defender</span><span class="sxs-lookup"><span data-stu-id="c7be8-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="c7be8-103">다음 단계에 따라 Microsoft Defender에서 서비스를 Office 365.</span><span class="sxs-lookup"><span data-stu-id="c7be8-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="c7be8-104">으로 이동하여 전역 관리자 또는 보안 관리자 [https://protection.office.com](https://protection.office.com) 계정으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="c7be8-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="c7be8-105">위협 관리의 왼쪽 탐색 **창에서** 정책 안전 **첨부** \> **파일을 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="c7be8-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="c7be8-106">에 **대해 Defender 켜기 를 Office 365,** SharePoint 및 OneDrive Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7be8-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="c7be8-107">[악의적인 파일을 감지할](/microsoft-365/compliance/create-activity-alerts) 때 알림을 받을 활동 경고 정책을 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="c7be8-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="c7be8-108">전체 지침은 에서 에 대해 안전한 첨부 파일 [SharePoint,](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)OneDrive 및 Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7be8-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="c7be8-109">**참고:** 기본적으로 Office 365 Microsoft Defender는 SharePoint Online, 비즈니스용 OneDrive 또는 Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7be8-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="c7be8-110">공유 활동, 게스트 활동 및 위협 신호를 사용하여 악성 파일을 식별하는 프로세스를 통해 파일을 비동기적으로 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="c7be8-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="c7be8-111">자세한 내용은 SharePoint, OneDrive 및 에 대한 안전한 첨부 [Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="c7be8-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
