 import java.util.Scanner; // importing scanner so it works in the program
class Assignment4trial4
{
    public static void main(String[] args)
    {
      int[] num = new int[3];
      Scanner in = new Scanner(System.in);
      System.out.println("please provide sides of a triangle give 000 to end program");
      for(int i = 0; i< 3; i++)
      {
        num[i] =  in.nextInt();// to keep collecting user input
      }
      
      equals(num);
     isosceles(num);
     isosceles2(num);
     isosceles3(num);
     scalene(num);
      endprogram(num);
    }
    public static void equals(int [] number)
    {
      if(number[0] == number[1] && number[1] == number[2])
      {
        System.out.println("It is an equalteral triangle");
      }
    }
    public static void isosceles(int[] number)
    {
      if( number[0] == number[1] && number[1] != number[2])
      {
        System.out.println("it is a isosceles triangle");
      }
    }
    public static void isosceles2(int[] number)
    {
      if( number[1] == number[2] && number[2] != number[0])
      {
        System.out.println("it is a isosceles triangle");
      }
    }
     public static void isosceles3(int[] number)
    {
      if( number[0] == number[2] && number[2] != number[1])
      {
        System.out.println("it is a isosceles triangle");
      }
    }
         public static void scalene(int[] number)
    {
      if( number[0] != number[1] && number[1] != number[2])
      {
        System.out.println("it is a scalene triangle");
      }
    }
         public static void endprogram (int[] number)
         {
             if(number[0] == 0 || number[1] ==0 ||  number[2] ==0)
      {
        System.out.println("the program has ended");
      }
         }
}
      
