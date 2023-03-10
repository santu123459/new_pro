# new_pro
1)  Write a Java program to swap two variables  
  
  public class SwapVariables {
   public static void main(String[] args) {
      int x = 10;
      int y = 20;
      System.out.println("Before Swapping: x = " + x + ", y = " + y);
      
      // Swapping Logic
      int temp = x;
      x = y;
      y = temp;
      
      System.out.println("After Swapping: x = " + x + ", y = " + y);
   }
}


2) Write a Java program to print the odd numbers from 1 to 20

public class PrintOddNumbers {
   public static void main(String[] args) {
      for (int i = 1; i <= 20; i++) {
         if (i % 2 != 0) {
            System.out.print(i + " ");
         }
      }
   }
}




3) Write a Java program to compute the sum of the first 100 prime numbers  


public class SumOfFirst100Primes {
   public static void main(String[] args) {
      int count = 0;
      int num = 2;
      int sum = 0;
      
      while (count < 100) {
         if (isPrime(num)) {
            sum += num;
            count++;
         }
         num++;
      }
      
      System.out.println("Sum of the first 100 prime numbers: " + sum);
   }
   
   public static boolean isPrime(int n) {
      if (n <= 1) {
         return false;
      }
      for (int i = 2; i <= Math.sqrt(n); i++) {
         if (n % i == 0) {
            return false;
         }
      }
      return true;
   }
}
    
    
    
    
    
4)Write a Java program to count the number of even and odd elements in a given array    
    

public class CountEvenAndOddElements {
   public static void main(String[] args) {
      int[] arr = {2, 4, 7, 8, 11, 14, 16, 19, 22};
      
      int countEven = 0;
      int countOdd = 0;
      
      for (int i = 0; i < arr.length; i++) {
         if (arr[i] % 2 == 0) {
            countEven++;
         } else {
            countOdd++;
         }
      }
      
      System.out.println("Number of even elements: " + countEven);
      System.out.println("Number of odd elements: " + countOdd);
   }
}







5) Write a Java program to add all the digits of a given positive integer

public class AddDigits {
   public static void main(String[] args) {
      int num = 12345;
      int sum = 0;
      
      while (num > 0) {
         int digit = num % 10;
         sum += digit;
         num /= 10;
      }
      
      System.out.println("Sum of digits: " + sum);
   }
}
