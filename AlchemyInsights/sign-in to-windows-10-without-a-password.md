---
title: 암호를 사용하지 않고 Windows 10에 로그인
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830552"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="b0fba-102">암호를 사용하지 않고 Windows 10에 로그인</span><span class="sxs-lookup"><span data-stu-id="b0fba-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="b0fba-103">Windows 시작 시 암호를 입력할 필요 없이 PIN, 얼굴 인식 또는 지문(사용 가능한 경우)과 같은 Windows Hello 보안 로그인 옵션 중 하나를 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="b0fba-104">보안 로그인을 사용하지 않도록 설정하려는 경우 아래 "Windows 10에 자동으로 로그인" 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b0fba-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="b0fba-105">**계정 암호 대신 Windows Hello 보안**</span><span class="sxs-lookup"><span data-stu-id="b0fba-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="b0fba-106">설정 > 계정 > **로그인 옵션으로** 이동합니다(또는 여기를 [클릭하십시오).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="b0fba-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="b0fba-107">사용 가능한 로그인 옵션이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="b0fba-108">예시:</span><span class="sxs-lookup"><span data-stu-id="b0fba-108">For example:</span></span>

![로그인 옵션.](media/sign-in-options.png)

<span data-ttu-id="b0fba-110">옵션 중 하나를 클릭하거나 탭하여 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="b0fba-111">다음에 Windows를 시작하거나 잠금을 해제하면 암호 대신 새 옵션을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="b0fba-112">**Windows 10에 자동으로 로그인**</span><span class="sxs-lookup"><span data-stu-id="b0fba-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="b0fba-113">**참고:** 자동 로그인은 편리하지만 특히 여러 사용자가 PC에 액세스할 수 있는 경우 보안 위험이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="b0fba-114">작업 표시줄에서 **시작** 단추를 클릭하거나 탭합니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="b0fba-115">**netplwiz를** 입력하고 Enter 키를 입력하여 사용자 계정 창을 여십시오.</span><span class="sxs-lookup"><span data-stu-id="b0fba-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="b0fba-116">사용자 **계정에서** Windows가 시작될 때 자동으로 로그인하려는 계정을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="b0fba-117">"사용자가 이 컴퓨터를 사용하려면 사용자 이름과 암호를 입력해야 합니다." 확인란의 선택을 선택하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![사용자는 사용자 이름 및 암호 옵션을 입력해야 합니다.](media/users-must-enter-username.png)

5. <span data-ttu-id="b0fba-119">**확인** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-119">Click **OK**.</span></span> <span data-ttu-id="b0fba-120">선택한 계정의 암호를 입력하고 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="b0fba-121">**확인** 을 클릭하여 작업을 마칩니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-121">Click **OK** to finish.</span></span> <span data-ttu-id="b0fba-122">다음에 Windows 10이 시작되면 선택한 계정에 자동으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="b0fba-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
