# NewRepo 
-----------------------------Array Example-----------------------------------------------------------

package mypackage;

public class Array {

	public static void main(String[] args) {
		
		
		//store age of patients
		int p1 = 10;
		int p2 = 33;
		int p3 = 35; 
		int p4 = 55; 
		int p5 = 65; 
		int p6 = 98;
		int p7 = 73;
		
		int patage[] = new int[7];
		
		patage[0] = 10;
		patage[1] = 33;
		patage[2] = 35;
		patage[3] = 55;
		patage[4] = 65;
		patage[5] = 98;
		patage[6] = 73;
		
		int i; 
		
		for (i=0; i<patage.length; i++){
			System.out.println("Value at index:"+i+"is:"+patage[i]);;
		}
		
		System.out.println("Length of array is : " + patage.length);

		Object obj[] = new Object[7]; // can accept all datatypes
		obj[0] = new Object [7];
		obj[0] =1;
		obj[1] ="Baba" ;
	}

}
------------------------------------------------Two Dimensional Array----------------------------------
package mypackage;

public class TwoDimensionalArray {

	public static void main(String[] args) {
		
	int a[][] = new int [3][3];
	
	//First Row
	a[0][0]= 0;
	a[0][1]= 3;
	a[0][2]= 0;
	a[1][0]= 3;
	a[1][1]= 0;
	a[1][2]= 3;
	a[2][0]= 0;
	a[2][1]= 3;
	a[2][2]= 3;
	
	int rowNum;
	int colNum;
	for (rowNum =0;rowNum<=2;rowNum++)
	{
		System.out.println("Row number is :" + rowNum);
	
	for(colNum = 0; colNum<=2; colNum++)
	{
		System.out.println(a[rowNum][colNum]);
	}
	}
	}
}

-----------------------------------Radio Button Example -----------------------------------------

package myPackage;


import java.util.List;
import java.util.concurrent.TimeUnit;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;

public class RadioButton {

	public static void main(String[] args) {
		
		WebDriver driver = new FirefoxDriver();
		driver.get("http://www.echoecho.com/htmlforms10.htm");
		driver.manage().window().maximize();
		driver.manage().timeouts().implicitlyWait(5, TimeUnit.SECONDS);
		List<WebElement> list =
		driver.findElements(By.xpath("//input[@name='group1']"));
		System.out.println(list.size());
		for(WebElement e:list){
		
	System.out.println(e.getAttribute("value"));
	System.out.println(e.isSelected());
	
		}
	}

}
