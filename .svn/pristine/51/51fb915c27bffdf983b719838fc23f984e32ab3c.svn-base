package com.nttdata.test;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.testng.annotations.Test;

public class NewTest {
  @Test
  public void AddBook(){
//	  WebDriver driver=new FirefoxDriver();
	  System.setProperty("webdriver.chrome.driver", "./Driver/chromedriver.exe");
	  WebDriver driver=new ChromeDriver();
	  driver.get("http://10.248.69.137:6080/ELibrary-Dev");
      driver.findElement(By.xpath("//form[@action='LibrarianLogin']/div/input[@id='email1']")).sendKeys("vanam.surendra@gmail.com");
      driver.findElement(By.xpath("//form[@action='LibrarianLogin']/div/input[@id='password1']")).sendKeys("Apr2017");
      driver.findElement(By.xpath("//form[@action='LibrarianLogin']//*[text()='Login']")).click();
      /*driver.findElement(By.xpath("//a[.='Add Book']")).click();
      driver.findElement(By.id("callno1")).sendKeys("123");
      driver.findElement(By.id("name1")).sendKeys("Java");
      driver.findElement(By.id("author1")).sendKeys("Surendra");
      driver.findElement(By.id("publisher1")).sendKeys("Sun Micro");
      driver.findElement(By.id("quantity1")).sendKeys("5");
      driver.findElement(By.xpath("//button[.='Save Book']")).click();*/
//	  driver.close();
      
      }
}
