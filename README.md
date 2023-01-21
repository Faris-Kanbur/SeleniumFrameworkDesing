# SeleniumFrameworkDesing

## In this test application, TestNG, Cucumber, Maven, Jebkins, page object design pattern were used and it was determined that logging in to the site in the process of purchasing a product, selecting the product and adding it to the basket, checking whether the product is in the basket, completing the purchase process of the product, and after purchasing the product, the transaction is successful. control is tested.

## To run this test, you can either use TestNG or run your test with Cucumber, or you can easily manage your process through Jenkins.

## You can run your test request via a browser (Chrome, Firefox, Edge) with the parameters you will send from Jenkins, or you can run it with the parameters you will send globally if you want.
Testinizde herhangi bir hata cikmasi durumunda bunu target dosyasi icinde hem ekran görüntüsü olarak hemde rapor olarak görebilir ve detayli bilgi alablirsiniz.


## Test Steps 
- Go to Login Page and Enter all data and click
- Select the product and go CartPage
- Check if it is on your product List
- Go to confirmation page
- And check all the buying process if succesful

## Compenent in Main Java

A -Abstract Compoennt

B: Pages :
  1-CartPage.java
  2-CheckOutPage.java
  3-Confirmation Page
  4-Landing Page
  5-Order Page
  6-Product Page
  
C:ExtentReporterNG
  1-GlobalDate.properties
  
## Compenent in Test Java

A-Cucumber
B-Academy
  1-data 
    a.DataReader.java
    b.PuchaseOrder.java
  2-stepDefinitions
  3-TestComponents
    a.BaseTest.java
    b.Listeners.java
    c.Retry.java
  4-test
    a.ErrorValidationsTest.java
    b.StandAloneTest.java
    c.SubmitOrderTest.java

## To run the tests

- mvn test -PTestName
- mvn test -Dbrowser=BrowserName
