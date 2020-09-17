---
title: 끝점 DLP 구성
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 406bc40fbe8a6306a2f74506ef1daf70b37283d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812121"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="1bbe6-102">끝점 DLP 구성</span><span class="sxs-lookup"><span data-stu-id="1bbe6-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="1bbe6-103">Microsoft 끝점 DLP를 사용하여 Windows 10 장치의 중요한 정보에 대한 DLP 보호 및 모니터링 기능을 확장할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="1bbe6-104">장치를 장치 관리에 등록한 후 DLP 정책을 만들어 항목에 보호 작업을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="1bbe6-105">활동 탐색기를 사용하여 중요한 항목의 활동을 모니터링할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="1bbe6-106">자세한 내용은 [장치 관리에 장치 등록](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="1bbe6-107">끝점 DLP를 시작하려면 다음을 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="1bbe6-108">해당 SKU/구독 라이선스가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="1bbe6-109">자세한 내용은 [SKU/구독 라이선스](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="1bbe6-110">장치 관리를 사용하도록 설정하고 등록 페이지에 액세스하거나 장치 모니터링을 설정/해제하는 데 필요한 권한을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="1bbe6-111">자세한 내용은 [사용 권한](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="1bbe6-112">장치 등록 절차를 따라 장치 관리에 장치를 등록합니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="1bbe6-113">M365 준수 **설정**에서 장치 등록(미리 보기) 옵션이 없는 경우에는 위에 참조된 적절한 라이선스 및 사용 권한을 보유하고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="1bbe6-114">자세한 내용은 [장치 등록](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="1bbe6-115">DLP 정책을 만들어 중요한 항목을 보호합니다.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="1bbe6-116">자세한 내용은 [끝점 DLP 정책 시나리오](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="1bbe6-117">Microsoft 끝점 DLP에 대한 자세한 내용은 [Microsoft 365 끝점 데이터 손실 방지(미리 보기) 알아보기](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1bbe6-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>