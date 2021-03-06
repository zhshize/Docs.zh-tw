---
title: ASP.NET Core MVC 與 Visual Studio 使用者入門
author: rick-anderson
description: 了解如何開始使用 ASP.NET Core MVC 與 Visual Studio。
ms.author: riande
ms.date: 10/07/2017
uid: tutorials/first-mvc-app/start-mvc
ms.openlocfilehash: 738c49272c2ae2b075866001f06ad09fe73969f9
ms.sourcegitcommit: 9bb58d7c8dad4bbd03419bcc183d027667fefa20
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2018
ms.locfileid: "52862196"
---
# <a name="get-started-with-aspnet-core-mvc-and-visual-studio"></a>ASP.NET Core MVC 與 Visual Studio 使用者入門

作者：[Rick Anderson](https://twitter.com/RickAndMSFT)

[!INCLUDE [consider RP](~/includes/razor.md)]

本教學課程有 3 個版本：

* macOS：[使用 Visual Studio for Mac 建立 ASP.NET Core MVC 應用程式](xref:tutorials/first-mvc-app-mac/start-mvc)
* Windows：[使用 Visual Studio 建立 ASP.NET Core MVC 應用程式](xref:tutorials/first-mvc-app/start-mvc)
* macOS、Linux 和 Windows：[使用 Visual Studio Code 建立 ASP.NET Core MVC 應用程式](xref:tutorials/first-mvc-app-xplat/start-mvc)

> [!NOTE]
> 我們正為規劃中的 ASP.NET Core 目錄新結構測試其可用性。  如果您有幾分鐘的時間可以嘗試在目前或建議的目錄中尋找 7 個不同主題，請[按一下這裡參加研究](https://dpk4xbh5.optimalworkshop.com/treejack/aa11wn82)。

## <a name="install-visual-studio-and-net-core"></a>安裝 Visual Studio 和 .NET Core

::: moniker range=">= aspnetcore-2.1"

[!INCLUDE [](~/includes/net-core-prereqs-windows.md)]

## <a name="create-a-web-app"></a>建立 Web 應用程式

從 Visual Studio 中，選取 [檔案] > [新增] > [專案]。

![[檔案] > [新增] > [專案]](start-mvc/_static/alt_new_project.png)

完成 [新增專案] 對話方塊：

* 在左窗格中，點選 [.NET Core]。
* 在中央窗格中，點選 [ASP.NET Core Web 應用程式 (.NET Core)]。
* 將專案命名為 "MvcMovie" (請務必將專案命名為 "MvcMovie"，以便複製程式碼時命名空間相符)。
* 點選 [確定]。

![[新增專案] 對話方塊, 左窗格中的 .Net core, ASP.NET Core Web ](start-mvc/_static/new_project2-21.png)

完成 [新增 ASP.NET Core Web 應用程式 (.NET Core) - MvcMovie] 對話方塊：

* 在版本選取器下拉式清單方塊中，選取 [ASP.NET Core 2.1]
* 選取 [Web 應用程式 (模型-檢視-控制器)]
* 點選 [確定]。

![[新增專案] 對話方塊, 左窗格中的 .Net core, ASP.NET Core Web ](start-mvc/_static/new_project22-21.png)

Visual Studio 在您剛才建立的 MVC 專案中使用了預設範本。 您只要輸入專案名稱，然後選取幾個選項，就立刻會有工作中的應用程式。 這是基本的入門專案，讓我們從這裡開始吧。

點選 **F5** 在偵錯模式中執行應用程式，或 **Ctrl-F5** 在非偵錯模式中執行。
<!-- These images are also used by uid: tutorials/first-mvc-app-xplat/start-mvc -->
![執行中的應用程式](start-mvc/_static/1.png)

* Visual Studio 會啟動 [IIS Express](/iis/extensions/introduction-to-iis-express/iis-express-overview)，並執行您的應用程式。 請注意，位址列會顯示 `localhost:port#`，而不是類似於 `example.com` 的內容。 這是因為 `localhost` 是本機電腦的標準主機名稱。 當 Visual Studio 建立 Web 專案時，會對網頁伺服器使用隨機連接埠。 在上圖中，連接埠號碼為 5000。 瀏覽器中的 URL 顯示`localhost:5000`。 當您執行應用程式時，會看到不同的連接埠編號。
* 使用 **Ctrl + F5** (非偵錯模式) 啟動應用程式，可讓您變更程式碼、儲存檔案、重新整理瀏覽器，以及查看程式碼變更。 許多開發人員想要使用非偵錯模式，以便快速啟動應用程式並檢視變更。
* 您可以從 [偵錯] 功能表項目的偵錯或非偵錯模式中啟動應用程式：

![[偵錯] 功能表](start-mvc/_static/debug_menu.png)

* 您可以點選 [IIS Express] 按鈕偵錯應用程式

![IIS Express](start-mvc/_static/iis_express.png)

預設範本提供您作用中的**首頁、關於**和**連絡人**連結。 上圖的瀏覽器不會顯示這些連結。 根據瀏覽器大小，您可能需要按一下巡覽圖示來顯示連結。

![右上角的瀏覽圖示](start-mvc/_static/2.png)

如果您在偵錯模式中執行，請點選 **Shift + F5** 停止偵錯。

在本教學課程的下一個部分中，我們會了解 MVC，並開始撰寫一些程式碼。

::: moniker-end

::: moniker range="<= aspnetcore-2.0"

[!INCLUDE [](~/includes/net-core-prereqs.md)]

## <a name="create-a-web-app"></a>建立 Web 應用程式

從 Visual Studio 中，選取 [檔案] > [新增] > [專案]。

![[檔案] > [新增] > [專案]](start-mvc/_static/alt_new_project.png)

完成 [新增專案] 對話方塊：

* 在左窗格中，點選 [.NET Core]。
* 在中央窗格中，點選 [ASP.NET Core Web 應用程式 (.NET Core)]。
* 將專案命名為 "MvcMovie" (請務必將專案命名為 "MvcMovie"，以便複製程式碼時命名空間相符)。
* 點選 [確定]。

![[新增專案] 對話方塊, 左窗格中的 .Net core, ASP.NET Core Web ](start-mvc/_static/new_project2.png)

完成 [新增 ASP.NET Core Web 應用程式 (.NET Core) - MvcMovie] 對話方塊：

* 在版本選取器下拉式清單方塊中，選取 [ASP.NET Core 2.-]。
* 選取 [Web 應用程式(模型檢視控制器)]。
* 點選 [確定]。

![[新增專案] 對話方塊, 左窗格中的 .Net core, ASP.NET Core Web ](start-mvc/_static/new_project22.png)

Visual Studio 在您剛才建立的 MVC 專案中使用了預設範本。 您只要輸入專案名稱，然後選取幾個選項，就立刻會有工作中的應用程式。 這是基本的入門專案，是個好開始。

點選 **F5** 在偵錯模式中執行應用程式，或 **Ctrl-F5** 在非偵錯模式中執行。
<!-- These images are also used by uid: tutorials/first-mvc-app-xplat/start-mvc -->
![執行中的應用程式](start-mvc/_static/1.png)

* Visual Studio 會啟動 [IIS Express](/iis/extensions/introduction-to-iis-express/iis-express-overview)，並執行您的應用程式。 請注意，位址列會顯示 `localhost:port#`，而不是類似於 `example.com` 的內容。 這是因為 `localhost` 是本機電腦的標準主機名稱。 當 Visual Studio 建立 Web 專案時，會對網頁伺服器使用隨機連接埠。 在上圖中，連接埠號碼為 5000。 瀏覽器中的 URL 顯示`localhost:5000`。 當您執行應用程式時，會看到不同的連接埠編號。
* 使用 **Ctrl + F5** (非偵錯模式) 啟動應用程式，可讓您變更程式碼、儲存檔案、重新整理瀏覽器，以及查看程式碼變更。 許多開發人員想要使用非偵錯模式，以便快速啟動應用程式並檢視變更。
* 您可以從 [偵錯] 功能表項目的偵錯或非偵錯模式中啟動應用程式：

![[偵錯] 功能表](start-mvc/_static/debug_menu.png)

* 您可以點選 [IIS Express] 按鈕偵錯應用程式

![IIS Express](start-mvc/_static/iis_express.png)

預設範本提供您作用中的**首頁、關於**和**連絡人**連結。 上圖的瀏覽器不會顯示這些連結。 根據瀏覽器大小，您可能需要按一下巡覽圖示來顯示連結。

![右上角的瀏覽圖示](start-mvc/_static/2.png)

如果您在偵錯模式中執行，請點選 **Shift + F5** 停止偵錯。

在本教學課程的下一個部分中，我們會了解 MVC，並開始撰寫一些程式碼。

::: moniker-end

> [!div class="step-by-step"]
> [下一步](adding-controller.md)  
