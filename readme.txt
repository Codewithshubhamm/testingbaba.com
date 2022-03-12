this is the sample file
created for jenkins
package arrayprogram;

import java.util.Scanner;

public class palindrome {
	public void getpailndrome(long mnum,long num)
	{
		
		String rev="";
		long temp=num;
		for(;mnum>0;)
		{
			long a = mnum%10;  
			  mnum = mnum/10;
			rev = rev+a;
			
		}
		int reverse =Integer.parseInt(rev);//it is used to break a string to int
		if(reverse==temp)
		{
			System.out.println(num+"is a pailendrome number:");
		}
		else
		{
			System.out.println(num+"is not a pailendrome");
		}				
	}
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		palindrome ob = new palindrome ();
		Scanner sc = new Scanner(System.in);
		System.out.println("type here the numbers");
		long num = sc.nextLong();
	    ob.getpailndrome(num, num);
	}

}
