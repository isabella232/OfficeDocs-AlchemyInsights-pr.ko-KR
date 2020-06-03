---
title: SharePoint 또는 OneDrive에서 항목을 삭제할 수 없음
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511982"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="ba074-102">항목을 삭제할 수 없음</span><span class="sxs-lookup"><span data-stu-id="ba074-102">Unable to delete items</span></span>

<span data-ttu-id="ba074-103">보존 정책에 의해이 문제가 발생 하는 해당 보류를 사용 하지 않도록 설정 하거나 제외 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ba074-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="ba074-104">보존 정책이 제거 된 후에는 변경 내용이 적용 되는 데 최대 24 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ba074-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="ba074-105">해당 항목에 대 한 [보존 정책](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) 설정이 없는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ba074-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="ba074-106">사이트의 저장 한도를 초과 하 여 사이트 [할당량](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) 을 높이 거 나 항목을 삭제 했을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ba074-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="ba074-107">항목이 다른 사용자에 게 [체크 아웃](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) 되지 않았는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ba074-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="ba074-108">마지막으로 관리자는 stubborn 항목 강제 삭제와 같은 복잡 한 관리 작업을 수행 하는 데 사용할 수 있는 PowerShell 명령 라이브러리가 포함 된 [SharePoint 패턴 및 사례](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP)를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ba074-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="ba074-109">PNP 파일 제거</span><span class="sxs-lookup"><span data-stu-id="ba074-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="ba074-110">PNP 폴더 제거</span><span class="sxs-lookup"><span data-stu-id="ba074-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="ba074-111">PNP 목록 항목 제거</span><span class="sxs-lookup"><span data-stu-id="ba074-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="ba074-112">PNP 목록 제거</span><span class="sxs-lookup"><span data-stu-id="ba074-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="ba074-113">PNP 필드 제거 (열)</span><span class="sxs-lookup"><span data-stu-id="ba074-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)