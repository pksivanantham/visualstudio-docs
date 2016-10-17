---
title: "Analyzing Load Test Virtual User Activity in the Details View of the Load Test Analyzer"
ms.custom: na
ms.date: 10/03/2016
ms.prod: visual-studio-tfs-dev14
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 63f4bd42-3cfb-4eee-af68-e8334976539e
caps.latest.revision: 22
manager: douge
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# Analyzing Load Test Virtual User Activity in the Details View of the Load Test Analyzer
**Virtual User Activity Chart**  
  
 ![Virtual User Activity Chart](../dv_TeamTestALM/media/Virtual_ActChart.png "Virtual_ActChart")  
  
 The Details view displays the Virtual User Activity Chart, which is used to visually analyze what the individual virtual users did during the load test. Virtual User Activity Chart lets you see patterns of user activity, load patterns, correlate failed or slow tests, and see requests with other virtual user activity. The Virtual User Activity Chart can also help you determine spikes in CPU usage, drops in requests per second, and what tests or pages were running during the spikes and drops.  
  
 **Requirements**  
  
-   Visual Studio Enterprise  
  
> [!NOTE]
>  Before you run the load test for which you want to use the Virtual User Activity Details Chart, you must verify that the **Timing Details Storage** property is set to the **AllIndividualDetails** option by using the Load Performance Test Editor. For more information, see [How to: Configure Collecting Full Details to Enable the Virtual User Activity Chart](../dv_TeamTestALM/How-to--Configure-Load-Tests-to-Collect-Full-Details-to-Enable-Virtual-User-Activity-in-Test-Results.md).  
  
 **Details Legend Panel**  
  
 ![Details legend panel](../dv_TeamTestALM/media/LTest_DetailsLegend.png "LTest_DetailsLegend")  
  
 The details legend panel is visible in the Virtual User Activity Chart. The details legend pane lets you filter out tests, pages and transactions based on several different criteria. For example, you can remove certain tests from the view, or remove all successful tests, or remove tests which failed with certain failures. You can also remove all tests that do not have logs.  
  
 You can highlight tests which failed, which displays all failed tests colored in red. You can also highlight tests that have test logs. Tests with logs will be colored in green.  
  
 **Filter results Panel**  
  
 ![Filter results panel](../dv_TeamTestALM/media/LTest_FilterResults.png "LTest_FilterResults")  
  
 The Filter results panel is visible in the Virtual User Activity Chart. The Filter results panel can filter on the following:  
  
-   **Show only results with logs** Displays only test results that have test logs associated with them.  
  
-   **Show successful results** Displays successful results.  
  
-   **Show results with errors** Displays results with errors that can help in debugging.  
  
## Tasks  
  
|Tasks|Associated topics|  
|-----------|-----------------------|  
|**Create a load test:** Before you analyze virtual user activity data in the test results of a load test, you must first create a load test.|-   [Creating and Editing Load and Web Performance Tests](assetId:///a3e3e7e6-46fc-45b1-b999-f461773f071b)|  
|**Configure your load test to use the Virtual User Activity Chart:** Before you run a load test that you want to view virtual user activity data on, you must first configure your load tests property settings.|-   [How to: Configure Collecting Full Details to Enable the Virtual User Activity Chart](../dv_TeamTestALM/How-to--Configure-Load-Tests-to-Collect-Full-Details-to-Enable-Virtual-User-Activity-in-Test-Results.md)|  
|**Run your load test:** After you have created a load test and configured it to enable virtual user activity data collecting, you must run the test until it is complete in order to view the Virtual User Activity Chart.|-   [Running Load Tests](../Topic/Running%20Load%20Tests.md)|  
|**View the load test results that contain the virtual user activity data:** After your load test has been created, configured, and has completed running, you can view the virtual user activity data by using the Virtual User Activity Chart.|-   [Analyzing Load Test Results](../dv_TeamTestALM/Analyzing-Load-Test-Results-Using-the-Load-Test-Analyzer.md)<br />-   [How to: Analyze What Virtual Users Are Doing During a Load Test](../dv_TeamTestALM/How-to--Analyze-What-Virtual-Users-Are-Doing-During-a-Load-Test-Using-the-Virtual-User-Activity-Chart.md)|  
|**Isolate performance issues in load tests:** You can use the Virtual User Activity Chart to help isolate performance issues in your load test.|-   [Walkthrough: Using the Virtual User Activity Chart to Isolate Issues](../dv_TeamTestALM/Walkthrough--Using-the-Virtual-User-Activity-Chart-to-Isolate-Issues.md)|  
  
## See Also  
 [Analyzing Load Test Results](../dv_TeamTestALM/Analyzing-Load-Test-Results-Using-the-Load-Test-Analyzer.md)   
 [Analyzing Load Test Results and Errors in the Tables View](../dv_TeamTestALM/Analyzing-Load-Test-Results-and-Errors-in-the-Tables-View-of-the-Load-Test-Analyzer.md)