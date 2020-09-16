---
title: Teams 관리 센터
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670370"
---
# <a name="teams-admin-center"></a><span data-ttu-id="aa4b4-102">Teams 관리 센터</span><span class="sxs-lookup"><span data-stu-id="aa4b4-102">Teams Admin Center</span></span>

<span data-ttu-id="aa4b4-103">[Teams 관리 센터](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)를 이용하여 Teams를 관리하는 방법을 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="aa4b4-104">Teams 관리 센터에 액세스할 수 없는 경우, 다음 항목을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="aa4b4-105">모든 주변 장치(방화벽 등) 혹은 로컬 컴퓨터의 방화벽 규칙에 적절한 [Office 365 IP 주소와 URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)을 허용했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="aa4b4-106">Teams 관리 포털에 액세스하는 데 사용 중인 로그인이 [Microsoft 365 관리 포털](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)에 나열된 사용자 이름과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="aa4b4-107">Teams 관리 센터에 사용자가 나타나지 않는 경우, 다음 항목을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="aa4b4-108">최근 24시간 동안 사용자를 만들었거나 라이선스를 할당했나요?</span><span class="sxs-lookup"><span data-stu-id="aa4b4-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="aa4b4-109">반드시 지원 티켓을 열기 전 최소한 24시간을 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="aa4b4-110">적절한 라이선스를 할당했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="aa4b4-111">온-프레미스 Active Directory를 가지고 있다면, [현지 Active Directory에 있는 ProxyAddresses 필드의 msRTCSIP-PrimaryUserAddress 또는 SIP 주소값이 고유하고, 형식이](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) [Microsoft 365 관리 센터](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)의 사용자 sip:**Username**과 일치하는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="aa4b4-112">비즈니스용 Skype 서버 배포를 유지하고 사용자가 온-프레미스와 온라인에 속하도록 하려면, 비즈니스용 Skype 서버 제어판에서 **"Teams와 비즈니스용 Skype 온라인을 하이브리드로 설정"** 을 참고하고 사용자를 온라인으로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="aa4b4-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
