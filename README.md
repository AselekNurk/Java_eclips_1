# Java_eclips_1
репозиторий для программ на java
import java.awt.*;
import java.util.Scanner;


public class Zad2_2 {
	public static void main(String []args){
		Scanner sc = new Scanner (System.in);
		int n;
		System.out.print("Введите количество студентов = ");
        n = sc.nextInt();
        int [] stud = new int [5];
        int kol_stud = 0,kol_o = 0;
    	for (int i=0; i<n; i++)
    	{kol_o=0;
    		System.out.println("Введите 5 оценок "+(i+1)+"-го студента: ");
    		
    		for (int j=0; j<5; j++)
    		{
    			stud[j] = sc.nextInt();
    		    if (stud[j]==2 || stud[j]==3)
    			kol_o++; 
    		}
    		if (kol_o==0) kol_stud++; 
    	}
    	 	
    	System.out.print(" Количество студентов не имеющих оценки 2 и 3 = "+kol_stud);  	
    	
	}
	
}
