---
title: SharePoint Online 시작
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700713"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="a8845-102">SharePoint의 워크플로</span><span class="sxs-lookup"><span data-stu-id="a8845-102">Workflows in SharePoint</span></span>

<span data-ttu-id="a8845-103">SharePoint 워크플로에서 전자 메일을 보내지 않는 경우 조직에서 Exchange Online 보낸 사람 제한이 발생 했을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a8845-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="a8845-104">다음 항목 중 하나가 있는 경우 ' 워크플로 일시 중단 ' 오류 메시지가 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a8845-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="a8845-105">Sharepoint Online의 워크플로를 사용 하 2013 2010 고 있으며,이를 수행 하는 사용자</span><span class="sxs-lookup"><span data-stu-id="a8845-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="a8845-106">워크플로는 한 번에 200 명 이상의 사용자에 게 사용자 지정 전자 메일 메시지를 전송 하거나, 하루에 1만 명의 받는 사람을 초과 하거나, 분당 30 개 이상의 메시지를 보내도록 구성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a8845-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="a8845-107">워크플로를 실행 하는 경우 전자 메일 메시지가 전송 되지 않으며, 내부 상태가 일시 중단 됨 또는 받는 사람에 게 보낼 수 없음으로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a8845-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="a8845-108">자세한 내용은 다음 [문서](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a8845-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

