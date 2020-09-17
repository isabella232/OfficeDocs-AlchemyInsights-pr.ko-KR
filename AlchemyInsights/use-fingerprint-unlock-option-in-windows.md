---
title: Windows 10에서 지문 잠금 해제 옵션 사용
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795250"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="845ed-102">Windows 10에서 지문 잠금 해제 옵션 사용</span><span class="sxs-lookup"><span data-stu-id="845ed-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="845ed-103">**Windows Hello 지문 사용**</span><span class="sxs-lookup"><span data-stu-id="845ed-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="845ed-104">지문을 사용 하 여 Windows 10의 잠금을 해제 하려면 windows Hello 지문을 추가 하 고 (Windows에서 인식할 수 있도록 허용) 하나 이상의 손가락을 설치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="845ed-105">**로그인 옵션 > 설정 > 계정** 으로 이동 하거나 [여기](ms-settings:signinoptions?activationSource=GetHelp)를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="845ed-106">사용 가능한 로그인 옵션이 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="845ed-107">예시:</span><span class="sxs-lookup"><span data-stu-id="845ed-107">For example:</span></span>

    ![로그인 옵션](media/sign-in-options.png)

2. <span data-ttu-id="845ed-109">**Windows Hello 지문을**클릭 하거나 탭 한 다음 **설정을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="845ed-110">Windows Hello 설정 창에서 **시작**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="845ed-111">지문 센서가 정품 인증 되며 손가락을 센서에 배치 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![지문 센서입니다.](media/fingerprint-sensor.png)

3. <span data-ttu-id="845ed-113">손가락을 반복적으로 검사 하는 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="845ed-114">이 작업이 완료 되 면 로그인에 사용할 다른 손가락을 추가할 수 있는 옵션이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="845ed-115">다음 번에 Windows 10에 로그인 할 때 지문을 사용 하 여이 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="845ed-116">**로그인 옵션으로 Windows Hello 지문을 사용할 수 없음**</span><span class="sxs-lookup"><span data-stu-id="845ed-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="845ed-117">**로그인 옵션**에서 Windows Hello 지문이 옵션으로 표시 되지 않는 경우 WINDOWS는 pc에 연결 된 지문 판독기/스캐너를 인식 하지 않거나 시스템 정책에 따라 사용을 차단 하는 경우 (예를 들어, PC가 회사에서 관리 하는 경우)에는 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="845ed-118">해결 방법:</span><span class="sxs-lookup"><span data-stu-id="845ed-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="845ed-119">작업 표시줄에서 **시작** 단추를 선택 하 고 **장치 관리자**를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="845ed-120">**장치 관리자**를 클릭 하거나 탭 하 여 엽니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="845ed-121">장치 관리자에서 해당 갈매기형 펼침 단추를 클릭 하 여 생체 인식 장치를 확장 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![생체 인식 장치](media/biometric-devices.png)

4. <span data-ttu-id="845ed-123">지문 스캐너가 Synaptics WBDI 스캐너와 같은 생체 인식 장치로 나열 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![생체 인식 장치](media/biometric-devices-expanded.png)

5. <span data-ttu-id="845ed-125">지문 스캐너가 표시 되지 않고 스캐너가 PC에 통합 되어 있는 경우 PC 제조업체의 웹 사이트로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="845ed-126">PC 모델의 기술 지원 섹션에서 설치할 수 있는 스캐너용 Windows 10 드라이버를 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="845ed-127">스캐너가 PC와 별개인 경우 (USB를 통해 연결 됨) 스캐너 제조업체의 웹 사이트로 이동 하 여 검색 프로그램 모델에 대 한 Windows 10 장치 드라이버 소프트웨어를 찾아서 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="845ed-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
