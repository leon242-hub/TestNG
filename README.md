    w testNG kiedy chcemy odpalić test z adnotacją @Test a mamy w innej klasie
    metodę z adnotacją np. @BeforeTest to ta metoda sie nie wykona.
     Musimy albo:
     1. Mieć wszystko w jednej klasie
     2. Albo rozszerzyć klase z ktora ma metodę z adnotacją @BeforeTest
     3. Albo odpalić z testng.xml -> ale tutaj będzie działać tylko @BeforeTest i @BeforeSuite



błąd Invalid Status code=403 text=Forbidden można naprawić dodając:

ChromeOptions options = new ChromeOptions();
options.addArguments("--remote-allow-origins=*");
