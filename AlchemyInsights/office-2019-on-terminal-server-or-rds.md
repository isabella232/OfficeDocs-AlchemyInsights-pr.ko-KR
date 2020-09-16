---
title: 터미널 서버 또는 RDS의 Office 2019
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3487"
- "9001419"
ms.openlocfilehash: 5454fad58411e9d86e19dfa83a1a553a2c2b05b4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47754571"
---
# <a name="deploying-office-2019-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="46b6a-102">RDS, 터미널 서버 또는 VDI에서 공유에 사용 하기 위한 Office 2019 배포</span><span class="sxs-lookup"><span data-stu-id="46b6a-102">Deploying Office 2019 for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="46b6a-103">Office가 다른 Office 계획을 사용 하 여 이미 RDS 서버에 설치 되어 있는 경우에는 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="46b6a-103">If Office is already installed on the RDS server using any other Office plans, uninstall it.</span></span> <span data-ttu-id="46b6a-104">예를 들어 제어판에서 **Control Panel**  >  **프로그램 제거**로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="46b6a-104">For example, go to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="46b6a-105">문제가 발생 하는 경우 [Microsoft 지원 및 복구 도우미](https://aka.ms/SARA-OfficeUninstall-Alchemy)를 사용 하 여 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="46b6a-105">If you're experiencing issues, uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span> 

<span data-ttu-id="46b6a-106">ODT (Office 배포 도구)를 사용 하 여 Office를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="46b6a-106">Use the Office Deployment Tool (ODT) to install Office.</span></span> <span data-ttu-id="46b6a-107">자세한 단계는 [Deploy Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="46b6a-107">For detailed steps, see [Deploy Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span></span>

<span data-ttu-id="46b6a-108">정품 인증에 대 한 자세한 내용은 [볼륨 정품 인증 Office의 개요](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="46b6a-108">For activation, see [Overview of volume activation of Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span></span>