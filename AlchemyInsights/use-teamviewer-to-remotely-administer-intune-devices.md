---
title: TeamViewer를 사용하여 Intune 장치 원격 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505212"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="82a65-102">TeamViewer를 사용하여 Intune 장치 원격 관리</span><span class="sxs-lookup"><span data-stu-id="82a65-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="82a65-103">Intune에서 관리하는 장치는 [TeamViewer](https://www.teamviewer.com/)를 사용하여 원격으로 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="82a65-104">TeamViewer를 사용하여 Intune을 관리하려면 다음 단계를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="82a65-105">먼저 TeamViewer에서 자격 증명을 가져와서 시작하여 Intune에서 TeamViewer 커넥터를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="82a65-106">이렇게 하면 관리자가 TeamViewer 커넥터 UI의 장치 아래에 자격 증명을 입력하고, 한 번의 작업으로 Intune과 TeamViewer 서비스 간에 연결을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="82a65-107">**1부: 원격 장치를 사용하여 세션 시작**</span><span class="sxs-lookup"><span data-stu-id="82a65-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="82a65-108">**모든 장치**에서 원격 세션을 시작하려는 장치를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="82a65-109">**...추가**에서 **새 원격 지원 세션**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="82a65-110">원격 세션 설정을 승인하려면 **예**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="82a65-111">TeamViewer 서비스에서 "새 원격 세션 시작" 요청을 승인하고 나면, 장치의 개요(또는 필수) 세부 정보 창 아래에서 **원격 지원 시작** 옵션이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="82a65-112">창을 확장하고 원격 지원 상태를 표시하려면 **더 보기**를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="82a65-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="82a65-113">**원격 세션 시작**을 선택하여 관리자 측에서 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="82a65-114">TeamViewer 바이너리(Windows)를 다운로드하도록 선택하고 **실행**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="82a65-115">**참고** TeamViewer 웹 사이트에 열린 모든 웹 브라우저 페이지를 무시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="82a65-116">TeamViewer 앱에 대한 요청을 승인하여 장치(Windows만 해당)에 대해 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="82a65-117">TeamViewer 앱이 시작되며 원격 장치에 대한 연결을 인증하기 위한 세션 코드를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="82a65-118">**2부: 원격 세션을 대상으로 하는 장치에서**</span><span class="sxs-lookup"><span data-stu-id="82a65-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="82a65-119">Intune 회사 포털을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="82a65-120">"IT 관리자가 원격 지원 세션에서 이 장치의 제어권을 요청하고 있습니다."라는 알림 플래그를 찾고 해당 알림을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="82a65-121">TeamViewer 응용 프로그램을 다운로드하도록 선택하거나 App Store에서 TeamViewer 앱 다운로드를 승인하고 **실행**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="82a65-122">**참고** TeamViewer 웹 사이트에 열린 모든 웹 브라우저 페이지를 무시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="82a65-123">TeamViewer 앱에 대한 요청을 승인하여 장치(Windows만 해당)에 대해 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="82a65-124">TeamViewer 앱이 시작되며 원격 장치에 대한 연결을 인증하기 위한 세션 코드를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="82a65-125">세션을 시작할 것인지 묻는 팝업이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="82a65-126">**참고** TeamViewer 서비스에서 생성되는 세션 코드는 일회용입니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="82a65-127">연결이 끊긴 경우 다음을 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="82a65-128">원격 장치 및 관리자 워크스테이션에서 TeamViewer 앱의 인스턴스를 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="82a65-129">원격 장치에서 회사 포털을 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="82a65-130">관리자 포털에서 "새 원격 지원 세션"을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="82a65-131">새 알림을 받으려면 원격 장치에서 회사 포털을 다시 엽니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="82a65-132">이전과 마찬가지로, 원격 장치와 관리자 워크스테이션에서 TeamViewer 앱을 다운로드하고 엽니다.</span><span class="sxs-lookup"><span data-stu-id="82a65-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>