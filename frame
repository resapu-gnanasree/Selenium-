package Package1;

import java.util.List;
import java.util.concurrent.TimeUnit;

import org.junit.After;
import org.junit.Before;
import org.junit.BeforeClass;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.Select;
import org.openqa.selenium.support.ui.WebDriverWait;

public class Demo10 {

	WebDriver driver;
	String url = "https://letcode.in/frame";

	@Before
	public void setUp() {
		// Set the key/value property according to the browser you are using.
		System.setProperty("webdriver.chrome.driver",
				"C:\\Software Testing Jars\\Drivers\\Chromedriver\\chromedriver.exe");

		// Open browser instance
		driver = new ChromeDriver();

		// Open the AUT
		driver.get(url);
		driver.manage().window().maximize();
		

	}

	@Test
	public void test() throws InterruptedException {
	
		driver.switchTo().frame("firstFr");
		driver.switchTo().frame(1);
		driver.findElement(By.name("email")).sendKeys("aaaaaa123@gmail.com");
		driver.switchTo().parentFrame();
		driver.findElement(By.name("fname")).sendKeys("777777777");
		Thread.sleep(10000);
		
	}

	@After
	public void tearDown() {
		// Close the browser
		driver.quit();
	}
}
