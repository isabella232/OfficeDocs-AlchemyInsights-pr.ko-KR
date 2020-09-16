---
title: 암호를 사용 하지 않고 Windows 10에 로그인
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719959"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="0953d-102">암호를 사용 하지 않고 Windows 10에 로그인</span><span class="sxs-lookup"><span data-stu-id="0953d-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="0953d-103">Windows 시작 시 암호를 입력 하지 않으려면 PIN, 얼굴 인식 또는 지문 같은 Windows Hello 보안 로그인 옵션 중 하나를 사용 하는 것이 좋습니다 (사용 가능한 경우).</span><span class="sxs-lookup"><span data-stu-id="0953d-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="0953d-104">보안 로그인을 실제로 사용 하지 않으려면 아래의 "Windows 10에 자동으로 로그인" 지침을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="0953d-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="0953d-105">**계정 암호 대신 Windows Hello 보안 대안을 적용할 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="0953d-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="0953d-106">**로그인 옵션 > 설정 > 계정** 으로 이동 하거나 [여기](ms-settings:signinoptions?activationSource=GetHelp)를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="0953d-107">사용 가능한 로그인 옵션이 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="0953d-108">예시:</span><span class="sxs-lookup"><span data-stu-id="0953d-108">For example:</span></span>

![로그인 옵션](media/sign-in-options.png)

<span data-ttu-id="0953d-110">옵션 중 하나를 클릭 하거나 탭 하 여 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="0953d-111">다음 번에 Windows를 시작 하거나 잠금 해제할 때 암호 대신 새로 만들기 옵션을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="0953d-112">**자동으로 Windows 10에 로그인**</span><span class="sxs-lookup"><span data-stu-id="0953d-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="0953d-113">**참고**: 자동 로그인은 편리 하지만, 특히 PC가 여러 사용자가 액세스할 수 있는 경우에는 보안 위험을 야기 합니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="0953d-114">작업 표시줄에서 **시작** 단추를 클릭 하거나 탭 합니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="0953d-115">**Netplwiz** 를 입력 하 고 Enter 키를 눌러 사용자 계정 창을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="0953d-116">**사용자 계정**에서 Windows가 시작 될 때 자동으로 로그인 할 계정을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="0953d-117">"사용자가이 컴퓨터를 사용할 수 있는 사용자 이름과 암호를 입력 해야 합니다." 확인란의 선택을 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![사용자가 사용자 이름 및 암호를 입력 해야 합니다.](media/users-must-enter-username.png)

5. <span data-ttu-id="0953d-119">**확인**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-119">Click **OK**.</span></span> <span data-ttu-id="0953d-120">선택한 계정에 대 한 암호를 입력 하 고 확인 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="0953d-121">**확인**을 클릭하여 작업을 마칩니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-121">Click **OK** to finish.</span></span> <span data-ttu-id="0953d-122">다음 번에 Windows 10을 시작 하면 선택한 계정에 자동으로 로그인 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0953d-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
