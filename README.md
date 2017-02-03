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
      //call for angle
      //angles (num);
     isosceles(num);
     //call for angle
     isosceles2(num);
     // call for angle
     isosceles3(num);
    // call for angle
     scalene(num);
    // call for angle
      endprogram(num);
    }
    public static void equals(int [] number)
    {
      if(number[0] == number[1] && number[1] == number[2])
      {
        System.out.println("It is an equalteral triangle");
        int  a = (int)Math.acos((Math.pow(number[0], 2) + Math.pow(number[1], 2) + Math.pow(number[2], 2)) / (2 * number[1] * number[2]));
        int  b = (int)Math.acos((Math.pow(number[1], 2) + Math.pow(number[0], 2) + Math.pow(number[2], 2)) / (2 * number[0] * number[2]));
        int  c = (int)Math.acos((Math.pow(number[2], 2) + Math.pow(number[0], 2) + Math.pow(number[1], 2)) / (2 * number[0] * number[1]));
        
          if (a > b && b > c)
          {
            if(a == 90)
            {
              System.out.println("it is a right trangle");
            }
          }
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
      //  public static void angles(int[] number)
    //   {
        //int  a = (int)Math.acos((Math.pow(number[0], 2) + Math.pow(number[1], 2) + Math.pow(number[2], 2)) / (2 * number[1] * number[2]));
      //  int  b = (int)Math.acos((Math.pow(number[1], 2) + Math.pow(number[0], 2) + Math.pow(number[2], 2)) / (2 * number[0] * number[2]));
        //int  c = (int)Math.acos((Math.pow(number[2], 2) + Math.pow(number[0], 2) + Math.pow(number[1], 2)) / (2 * number[0] * number[1]));
       //   if (a > b && b > c)
         // {
          //  if(a == 90)
         //   {
       ///       System.out.println("it is a right trangle");
       //     }
       //   }
          
      //  }
         
         public static void endprogram (int[] number)
         {
             if(number[0] == 0 || number[1] ==0 ||  number[2] ==0)
      {
        System.out.println("the program has ended");
      }
         }
}
      
