---
title: 902(중복 개체로 인한 동기화 오류)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708068"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="3c287-102">중복 개체로 인한 동기화 오류</span><span class="sxs-lookup"><span data-stu-id="3c287-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="3c287-103">Microsoft 365에서 디렉터리 동기화가 완료되면 다음 오류 메시지 중 하나를 수신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3c287-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="3c287-104">이 개체와 연결된 다음 Microsoft Online Services 로컬 디렉터리의 다른 개체와 이미 연결되어 있을 수 있는 값이 있기 때문에 이 개체는 업데이트할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3c287-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="3c287-105">프록시 주소가 같은 동기화된 개체가 Microsoft Online Services 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3c287-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="3c287-106">이 개체와 연결된 다음 특성에는 로컬 디렉터리 서비스의 다른 개체와 이미 연결되어 있을 수 있는 값이 있기 때문에 이 개체를 업데이트할 수 없습니다. UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3c287-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="3c287-107">문제를 식별하고 해결하려면 [IdFix DirSync](https://github.com/Microsoft/idfix)오류 수정 도구를 다운로드하여 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="3c287-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="3c287-108">자세한 내용은 [KB2647098을 참조하세요.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="3c287-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
