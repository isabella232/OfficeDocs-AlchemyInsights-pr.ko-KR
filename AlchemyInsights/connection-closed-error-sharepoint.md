---
title: SharePoint의 기본 연결이 닫힘 오류
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 762b000fd9c63e0913a88402150055e8ee7c56de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505876"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="58fa6-102">SharePoint의 "기본 연결이 닫혀 있습니다" 오류</span><span class="sxs-lookup"><span data-stu-id="58fa6-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="58fa6-103">SharePoint에서 "기존 연결이 닫혔습니다"라는 오류가 표시될 경우, 이 문제는 TLS 1.0/1.1 사용 중단과 관련이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="58fa6-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="58fa6-104">자세한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="58fa6-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="58fa6-105">Office 365 및 Office 365 GCC에서 TLS 1.2 준비</span><span class="sxs-lookup"><span data-stu-id="58fa6-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="58fa6-106">클라이언트에 TLS 1.2가 지원되지 않는 경우 인증 오류 발생</span><span class="sxs-lookup"><span data-stu-id="58fa6-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)