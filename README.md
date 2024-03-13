import java.util.*;
public class Main 
{
    public static void main(String [] args) {
        Scanner in = new Scanner(System.in);
        int rem;
        int sum = 0;
        int sum1=0;
        int sum2=0;
        System.out.print("Enter the number :");
        int a = in.nextInt();
        System.out.print("Enter the number of time :");
        int b = in.nextInt();
        while(a>0)
        {
            rem=a%10;
            sum=sum+rem;
            a=a/10;
        }
        sum=sum*b;
        while(sum>0){
            rem=sum%10;
            sum1=sum1+rem;
            sum=sum/10;
        }
          while(sum1>0){
            rem=sum1%10;
            sum2=sum2+rem;
            sum1=sum1/10;
            System.out.println("Final answer is :" +sum2);
        }
        
}
}
