# TestFramework
Demo framework using selenium and restsharp

*******How to Use Framework********
1. First create log directory as C>code>Logs
2. Download Demo.zip and extract in any directory lets say Under D:
3. Open TestAutomation.sln in visual studio 2019. Make sure .Net Framework available as 4.7.2
4. Build entire solution
5. Once solution build successfully. Open test explorer.
6. We should be able to see Two different test suite as testImage.png.
7. Selenium Test added in DemoTesting.cs class
8. API test using restsharp added under CrudOperationTests.cs
9. Run to check results.
10. Logs and screenshot will be created in this directory: C>code>Logs
11. Extent(HTML) report will be available under: <Source directory>:Demo\TestAutomation\SeleniumTestFramework\Report\index.html

******Further improvement required in Framework*********
  
For Selenium Test Framework:
  1. Extent report object can be instantiated in LogService.cs constructor and will be use across framework instead of only used in test class
  2. WebDriverBase.cs can contain other selenium actionable methods. Currently only require methods were added
  3. BaseClass.cs should have condition support to include condition if dev wants to run test cases in container
  4. Selenium actionable methods in WebDriverBase.cs should be under try/catch to store exception object and same would be useful to detect where exception has been originated

For API Test Framework:
  1. We can added Helper class to avoid duplicate codes witten in userservice.cs
  2. Logs and extent report features can be incorporated similar to selenium framework
  3. Model can have getter/setter classes similar to DTO to have set data in object instead of hardcoded.
