---
title: 如何閱讀您的帳單 & 偵察檔案
ms.topic: article
ms.date: 06/05/2020
description: 瞭解您的發票 & 對帳檔案。 您的帳單會針對該月期間的方案、產品和客戶顯示合作夥伴中心的費用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
keywords: 訂閱計費, 計費, 合作夥伴中心的計費, 合作夥伴中心計費, 閱讀帳單, 發票, 合作夥伴中心發票, CSP 發票, 我的帳單在哪裡？
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40809fbca8ed81882e9b1d315fd5967143faff1e
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949318"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>瞭解您的帳單和對帳檔案-瞭解如何在合作夥伴中心尋找

**適用於**

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

**適當的角色**

- 全域系統管理員
- 帳單系統管理員
- 系統管理代理人


您的**發票**是**所有合作夥伴中心費用的摘要**（跨方案、所有產品和所有客戶）。 

## <a name="invoice-types"></a>發票類型

Microsoft 會針對任何以授權為基礎的費用（例如，Office 365）和以使用量為基礎的費用（例如 Azure），或針對一次性費用（例如 Azure RI、Marketplace 或 Azure 方案）發出一份發票。

例如，  

**案例 1 [單一貨幣]**：合作夥伴已購買145P 供應專案和 O365 授權，  

- 合作夥伴會取得一個發票 PDF 和2個對帳檔案，其中涵蓋 O365 和 Azure （145p）的費用。  

**案例 2 [單一貨幣]**：合作夥伴已購買 azure RI、Marketplace 和/或 azure 方案以及145p 購買。

- 合作夥伴會收到一個發票 PDF 和一個涵蓋 Azure 費用的對帳檔案（145p）。 

- 合作夥伴會收到另一個發票 PDF 和對帳檔案，其中涵蓋 Azure RI、Marketplace、Azure 方案的費用。 

**案例 3 [多貨幣]**：合作夥伴已購買丹麥幣中的 azure RI 和以 eur 計算的 azure 方案及145p 購買歐元。

- 合作夥伴會收到一個發票 PDF 和對帳檔案，其中涵蓋丹麥幣中的 Azure RI 費用。 

- 合作夥伴會收到一個發票 PDF 和一個對帳檔案，其中涵蓋以 EUR 計算的 Azure 方案費用。 

- 合作夥伴將會收到另一個發票 PDF 和對帳檔案，其中涵蓋以 EUR （或合作夥伴計費貨幣）145p 供應專案的費用。 

## <a name="find-your-bill"></a>尋找帳單 

您可以在 [合作夥伴中心] 儀表板的 [帳單] 頁面上找到您的發票。 您也可以在此頁面上找到您的帳單歷程記錄、支出趨勢和對帳檔案。 

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。 

2. 在左側功能表中，選取 [ **帳單**]。 

3. 在 [帳單] 頁面上，選取您想要下載的發票。 

您可以在頁面頂端的 [帳戶餘額] 底下，找到最新發票的連結（最後一個發票日期）。 

您可以在 [帳單歷程記錄] 區段中找到先前的發票。 選擇適當的年份，然後選取適當計費週期旁的下拉箭號。 選取 [發票（.pdf）] 旁的連結，以下載該期間的發票。 

## <a name="understanding-invoice-pdf"></a>瞭解發票 PDF 

**使用量和授權型費用的發票**： Office 365 和 Azure 等服務費用的發票將會在您所選計費日期 [UTC] 的兩天內提供。  

**Onetime 和週期性費用的發票**： azure RI、azure 方案、Marketplace 等服務費用的發票將于每個月的第8天后提供。  

以下是發票 PDF 檔上的一些重要欄位–

**發票編號**：針對個別計費期間所產生發票檔的唯一識別碼。 

**計費週期**：這是您有使用方式和授權型服務的期間。 

**發票日期**：每個月產生發票的計費日期或週年日。 

**付款到期日**：必須收到付款的日期。 

**費用**：您的計費貨幣在個別計費週期中的到期金額。 

**信用額度**：對訂用帳戶所做之變更的信用額度（例如 SLA）或調整（例如，基座增加或減少）。 

**付款指示**：根據您的區域支付發票費用的說明。 付款時務必要包含您的發票號碼。 

如需發票檔案中所有欄位的詳細描述（包括一次性費用的欄位），請參閱 [發票檔案欄位](invoice-file.md)。 

## <a name="understand-reconciliation-files"></a>瞭解對帳檔案

 對帳檔案提供您費用的向下切入/詳細資料，可與發票 PDF 一起下載。 對帳檔案包含您可以用來建立客戶發票的客戶識別碼和訂用帳戶識別碼。 請參閱 [如何使用對帳](use-the-reconciliation-files.md)檔案，以取得更多有關偵察檔案的詳細資料。 
