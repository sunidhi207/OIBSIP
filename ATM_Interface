import java.util.*;
class Account_Details
{
	String name,userName,password,accountNo;
    float balance=100000;
	int transaction=0;
    String transactionHistory="";
    public void transaction_history()
    {
    	if(transaction==0)
    	{
    		System.out.println("Empty");
    	}
    	else
    	{
    		System.out.println(transactionHistory);
    	}
    }
    public void accountDetails()
    {
    	Scanner sc=new Scanner(System.in);
    	System.out.println("Enter your name: ");
    	name=sc.nextLine();
    	System.out.println("Enter your userName: ");
    	userName=sc.nextLine();
    	System.out.println("Enter your password: ");
    	password=sc.nextLine();
    	System.out.println("Enter your accountNo.=");
    	accountNo=sc.nextLine();
    	 }
    public void displayDetails()
    {
    	System.out.println("Account holder name is: "+name);
    	System.out.println("User name is: "+userName);
    	System.out.println("Password is: "+password);
    	System.out.println("Account holder name is: "+accountNo);
    	
    }
    public boolean login()
    {
    	boolean isLogin=false;
    	Scanner sc=new Scanner(System.in);
    	while(!isLogin)
    	{
    		System.out.println("Enter your user name to login account:");
    		String Username;
    		
    		Username=sc.nextLine();
    		if(Username.equals(userName))
    		{
    			while(!isLogin)
    			{
    				String Password;
    				System.out.println("Enter your password:");
    				Password=sc.nextLine();
    				if(Password.equals(password))
    				{
    					
    					System.out.println("Login Successful!!!");
    					isLogin=true;
    				}
    				else
    				{
    					System.out.println("Wrong password");
    				}
    		
    			}
    		
    	}
    		else
    		{
    			System.out.println("Invalid Username");
    		}

    }
    	return isLogin;
}
    public void deposit()
    {
    	Scanner sc=new Scanner(System.in);
    	System.out.println("Enter amount: ");
    	float amount=sc.nextInt();
    	
    	if(amount<=100000)
    	{
    		transaction++;
    		balance=balance+amount;
    		System.out.println(balance+" Rs deposited.");
    	}
    	else
    	{
    		 System.out.println("Limit can't exceed beyond 100000");
    		 
    	}
    	String str=""+balance;
    	transactionHistory=transactionHistory.concat(str);
    
    	}
    public void transfer()
    {
    	Scanner sc=new Scanner(System.in);
    	System.out.println("Enter the amount you want to withdrawal: ");
    	int withdrawal_amount;
    	withdrawal_amount=sc.nextInt();
    	if(balance>=withdrawal_amount)
    	{
    		if(balance>=1000)
    		{
    			transaction++;
    			balance=balance-withdrawal_amount;
    			System.out.println(balance+" Rs. is debited.");
    		}
    		else
    		{
    			System.out.println("Insufficient Balance");
    		}
    	}
    	else
    	{
    		System.out.println("Insufficient Balance");
    	}
    	String str=""+balance;
    	transactionHistory=transactionHistory.concat(str);
    }
}

    

public class Bank_Account {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Account_Details b=new Account_Details();
		Scanner sc=new Scanner(System.in);
		boolean isFinished=true;
		System.out.println("**********Welcome to ABC bank**********");
		System.out.println();
		b.accountDetails();
		if(b.login())
		{
		while(isFinished!=false)
		
		{
		System.out.println("Enter your choice: \n 1* Display Account details \n 2* deposit \n 3* withdraw \n 4* Transaction history. ");
        int c=sc.nextInt();
        switch(c)
        {
        case 1:b.displayDetails();
               break;
        case 2:b.deposit();
                break;
        case 3:b.transfer();     
                break;
        case 4:b.transaction_history();   
                break;
        default:isFinished=false; 
        }
	}
		}
	}

}
