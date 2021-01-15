---
title: 如何讀取帳單 & 偵察檔
ms.topic: article
ms.date: 06/05/2020
description: 深入瞭解您的發票 & 對帳檔案。 您的帳單會顯示該月期間內的方案、產品和客戶合作夥伴中心費用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43c2605d750d35bc2e0095b1fed413ed91a1a28e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215810"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>瞭解您的帳單和對帳檔案-瞭解如何在合作夥伴中心中尋找


**適當的角色**

- 全域系統管理員
- 帳單系統管理員
- 系統管理代理人


您的 **發票** 是 **所有合作夥伴中心費用的摘要** ， (整個方案、所有產品和所有客戶) 。 

## <a name="invoice-types"></a>發票類型

Microsoft 會針對任何以授權為基礎的費用發出一張發票 (例如，Office 365) 和以使用量為基礎的費用 (例如 Azure) ，以及針對一次性費用的個別發票 (例如 Azure RI、Marketplace 或 Azure 方案) 。

例如，  

**案例 1 [單一貨幣]**：合作夥伴已購買145P 供應專案和 O365 授權  

- 合作夥伴會取得一個發票 PDF 和2個對帳檔案，其中涵蓋 O365 和 Azure (145p) 的費用。  

**案例 2 [單一貨幣]**：合作夥伴已購買 azure RI、Marketplace 及/或 azure 方案，以及145p 購買。

- 合作夥伴會取得一個發票 PDF，以及涵蓋 Azure (145p) 費用的對帳檔案。 

- 合作夥伴會收到另一個發票 PDF 和一個對帳檔案，其中涵蓋其 Azure RI、Marketplace、Azure 方案的費用。 

**案例 3 [多貨幣]**：合作夥伴已在丹麥幣和 azure 方案中購買 azure RI 以及歐元的145p 購買。

- 合作夥伴會收到一個發票 PDF 和一個對帳檔案，其中涵蓋丹麥幣中 Azure RI 的費用。 

- 合作夥伴會收到一個發票 PDF，以及一個涵蓋 Azure 方案費用的對帳檔案（以歐元計算）。 

- 合作夥伴會收到另一個發票 PDF 和一個對帳檔案，其中涵蓋其145p 優惠的歐元 (或合作夥伴的帳單貨幣) 費用。 

## <a name="find-your-bill"></a>尋找帳單 

您可以在 [儀表板] 的 [帳單] 頁面中找到合作夥伴中心的發票。 您也可以在此頁面上找到您的帳單歷程記錄、支出趨勢和對帳檔案。 

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。 

2. 在左側功能表中，選取 [ **計費**]。 

3. 在 [帳單] 頁面上，選取您要下載的發票。 

您可以在頁面頂端的 [帳戶餘額] 下的 [上次發票日期] 中找到最新發票的連結。 

您可以在 [帳單記錄] 區段中找到先前的發票。 選擇適當的年份，然後選取適當計費週期旁的下拉式箭號。 選取發票 ( .pdf) 旁的連結，以下載該期間的發票。 

## <a name="understanding-invoice-pdf"></a>瞭解發票 PDF 

**使用量和以授權為基礎的費用發票**：適用于 Office 365 和 Azure 等服務費用的發票將于您所選計費日期的兩 (2) 天內提供 [UTC]。  

**Onetime 和週期性費用的發票**：服務的費用發票（例如 azure RI、azure 方案、Marketplace）將于每月的每月8日之後提供。  

以下是發票 PDF 檔上的一些索引鍵欄位–

**發票號碼**：針對個別計費期間所產生發票檔的唯一識別碼。 

**計費週期**：這是您使用使用方式和授權型服務的期間。 

**發票日期**：每個月產生發票的計費日期或週年日。 

**付款到期日**：必須收到付款的日期。 

**費用**：依計費期計費的帳單貨幣所應付的金額。 

**信用額度**：點數 (例如 SLA) 或對訂用帳戶所做的調整 (例如，授權增加或減少) 。 

**付款指示**：如何根據您的區域支付發票的說明。 付款時，務必要包含您的發票號碼。 

如需發票檔案中所有欄位的詳細描述 (包含一次性費用) 的欄位，請參閱 [發票檔案欄位](invoice-file.md)。 

## <a name="understand-reconciliation-files"></a>瞭解對帳檔案

 針對您的費用提供深入探討/詳述詳細資料的對帳檔案，可隨發票 PDF 下載。 對帳檔案包含客戶識別碼和訂用帳戶識別碼，您可以用來建立客戶的發票。 請參閱  [如何使用對帳](use-the-reconciliation-files.md) 檔案，以取得更多有關偵察檔案的詳細資料。 

## <a name="next-steps"></a>後續步驟

- [如何使用對帳檔案](use-the-reconciliation-files.md)