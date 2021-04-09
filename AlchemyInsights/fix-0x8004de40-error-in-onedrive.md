---
title: OneDrive에서 0x8004de40 오류 수정
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649754"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="04774-102">OneDrive에서 0x8004de40 오류 수정</span><span class="sxs-lookup"><span data-stu-id="04774-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="04774-103">Windows 7을 실행 중이고 이 오류가 발생하는 경우 [Windows의 WinHTTP에서 TLS 1.1 및 TLS 1.2를](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)기본 보안 프로토콜로 사용하도록 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="04774-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="04774-104">Windows 10을 실행 중일 때 OneDrive에 0x8004de40 오류가 발생하는 경우:</span><span class="sxs-lookup"><span data-stu-id="04774-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="04774-105">Acitve 디렉터리 도메인에 연결된 동안 영향을 받는 컴퓨터를 다시 시작하십시오.</span><span class="sxs-lookup"><span data-stu-id="04774-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="04774-106">다시 시작해도 문제가 해결되지 않는 경우 Azure AD에서 디바이스에 조인을 언 후 다시 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="04774-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="04774-107">**참고:** 이 단계를 수행하는 동안 회사 네트워크에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="04774-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="04774-108">회사 인프라에 연결되지 않은 경우(예: 출장 중) 이러한 단계를 수행하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="04774-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="04774-109">시작을 선택하여 관리자 권한 명령 프롬프트를 **열고** 명령 프롬프트를 마우스 오른쪽 단추로 **클릭한** 다음 관리자 권한으로 실행 **을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="04774-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="04774-110">*dsregcmd /leave를 입력하고* **Enter를 누르고 를 입력합니다.**</span><span class="sxs-lookup"><span data-stu-id="04774-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="04774-111">완료되면 *dsregcmd /join을 입력하고* **Enter를 누르고 를 입력합니다.**</span><span class="sxs-lookup"><span data-stu-id="04774-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="04774-112">완료되면 명령 프롬프트를 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="04774-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="04774-113">컴퓨터를 다시 시작하고 OneDrive에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="04774-113">Reboot the computer, and log into OneDrive.</span></span>