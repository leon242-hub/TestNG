    w testNG kiedy chcemy odpalić test z adnotacją @Test a mamy w innej klasie
    metodę z adnotacją np. @BeforeTest to ta metoda sie nie wykona.
     Musimy albo:
     1. Mieć wszystko w jednej klasie
     2. Albo rozszerzyć klase z ktora ma metodę z adnotacją @BeforeTest
     3. Albo odpalić z testng.xml -> ale tutaj będzie działać tylko @BeforeTest i @BeforeSuite



błąd Invalid Status code=403 text=Forbidden można naprawić dodając:

ChromeOptions options = new ChromeOptions();
options.addArguments("--remote-allow-origins=*");


JavascriptExecutor
execteScript and executeAsyncScript -> The function invoked with executeAsyncScript takes a 'done callback' as the last argument, which must be called to signal that the script is done executing. This allows it to be used with code that only 'finishes' when a callback is used - eg. setTimeout or asynchronous XHR.
