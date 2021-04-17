---
title: 계정 잠금 해제
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002449"
- "4748"
ms.openlocfilehash: 532b273154a31c024825b150d9b0edd42eb6130c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827762"
---
# <a name="unlocking-an-account"></a><span data-ttu-id="625be-102">계정 잠금 해제</span><span class="sxs-lookup"><span data-stu-id="625be-102">Unlocking an account</span></span>

<span data-ttu-id="625be-103">잘못된 암호 시도나 다른 손상으로 인해 Microsoft 365에서 사용자의 계정이 잠겼을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="625be-103">It's possible users are locked out of Microsoft 365 due to bad password attempts or other compromises.</span></span> <span data-ttu-id="625be-104">사용자가 Microsoft 365에 다시 로그인할 수 있게 하기 위해 **지원 요청을 열기 전에 다음 단계를 시도해 볼 수 있습니다**.</span><span class="sxs-lookup"><span data-stu-id="625be-104">To help users sign back in to Microsoft 365, **you can attempt the following steps before opening a Support Request**.</span></span> 

<span data-ttu-id="625be-105">**전자 메일 제한됨**</span><span class="sxs-lookup"><span data-stu-id="625be-105">**Email Restricted**</span></span>

<span data-ttu-id="625be-106">사용자 중 누군가 전자 메일을 보낼 수 없도록 제한이 된 경우, 관리자는 계정을 [직접 차단 해제](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="625be-106">As an admin, if one of your users is restricted from sending email, you can [unblock the account yourself](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam).</span></span> <span data-ttu-id="625be-107">사용자는 제한이 해제된 후 1시간 이내에 전자 메일을 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="625be-107">The user will be able to send email within an hour after removing the restriction.</span></span>

<span data-ttu-id="625be-108">**사용자 암호 재설정**</span><span class="sxs-lookup"><span data-stu-id="625be-108">**Reset the User Password**</span></span>

1. <span data-ttu-id="625be-109">관리 센터에서 **사용자 > [활성 사용자](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** 로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="625be-109">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="625be-110">사용자를 선택하고 **암호 재설정** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="625be-110">Select the user and click **Reset Password**.</span></span>

<span data-ttu-id="625be-111">**사용자가 로그인하도록 허용되었는지 확인**</span><span class="sxs-lookup"><span data-stu-id="625be-111">**Make sure the user is allowed to sign in**</span></span>

1. <span data-ttu-id="625be-112">관리 센터에서 **사용자 > [활성 사용자](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)** 로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="625be-112">In the admin center, go to **Users > [Active Users](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)**.</span></span>

2. <span data-ttu-id="625be-113">사용자를 선택하고 **추가 작업(...)** 을 클릭한 후 **로그인 상태 편집** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="625be-113">Select the user and click **More Actions (...)**; then click **Edit sign-in status**.</span></span>

<span data-ttu-id="625be-114">셀프 서비스 암호 재설정을 비롯한 더 많은 암호 재설정 시나리오는 [온라인 결제 수단으로 청구할 수 있는 다양한 시도를 위한Microsoft 365 Business 암호 재설정](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords?view=o365-worldwide)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="625be-114">For more password reset scenarios, including Self-Service Password Reset, see [Reset Microsoft 365 for multiple-attempts-to-charge-online-payment-instrumentsbusiness passwords](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords?view=o365-worldwide).</span></span>

<span data-ttu-id="625be-115">이 서비스는 손상된 계정 및/또는 스팸 발신의 증거를 감지하여 사용자가 전자 메일을 보내지 못하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="625be-115">The service prevents a user from sending email after detecting evidence of a compromised account and/or outbound spam.</span></span> <span data-ttu-id="625be-116">예방 조치로 사용자를 위해 [Microsoft 365에서 손상된 전자 메일 계정에 응답](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)의 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="625be-116">As a precaution, follow the steps in [Responding to a Compromised Email Account in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account) for the user.</span></span>
