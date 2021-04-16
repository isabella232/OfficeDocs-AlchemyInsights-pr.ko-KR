---
title: Microsoft 365 앱 수정 계정이 잘못된 상태 메시지에 있습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812542"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="8d171-102">Microsoft 365 앱 "계정이 잘못된 상태입니다." 오류 수정</span><span class="sxs-lookup"><span data-stu-id="8d171-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="8d171-103">이 오류를 해결하려면 영향을 받는 컴퓨터에서 다음 옵션을 시도해 보십시오.</span><span class="sxs-lookup"><span data-stu-id="8d171-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="8d171-104">Office 앱을 열고 파일  >  **계정에서** 모든  >  **계정에서 로그인을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="8d171-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="8d171-105">유효한 라이선스가 있는 사용자 계정을 사용하여 다시 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="8d171-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="8d171-106">자세한 내용은 [Office의 계정](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d171-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8d171-107">Windows [자격 증명 관리자를](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) 사용하여 Office 자격 증명 지우기</span><span class="sxs-lookup"><span data-stu-id="8d171-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="8d171-108">**참고:** Office 2016의 레지스트리 경로가 16.0으로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="8d171-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8d171-109">예를 들어 \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="8d171-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="8d171-110">Office 2013을 사용하여 Office 365에 연결하는 동안 오류가 발생하는 경우 Office 클라이언트에 대해 최신 [인증을](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 사용하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d171-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="8d171-111">자세한 내용은 [Microsoft 365, Azure 또는 Intune에](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)로그인할 수 없는 브라우저가 아닌 앱 문제를 해결하는 방법을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d171-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

