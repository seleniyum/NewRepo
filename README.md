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
