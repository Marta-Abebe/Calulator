# Calulator
Java Simple Calculator Coding
import java.util.Scanner;

public class SimpleCalculator  {
  public static void main(String[] args) {
 
    int Num1, Num2, Result;
    char operator;
   
    Scanner input = new Scanner(System.in);

    System.out.println("Choose an operator: +, -, *,  /, % : ");
    operator = input.next().charAt(0);

    System.out.println("Enter Num 1:");
    Num1 = input.nextInt();

    System.out.println("Enter Num 2: ");
    Num2 = input.nextInt();
    
//Get logic 
    switch (operator) {

    
      case '+':
        Result = Num1 +Num2;
        System.out.println(Num1 + " + " + Num2 + " = " + Result);
        break;

      case '-':
        Result = Num1 - Num2;
        System.out.println(Num1 + " - " + Num2 + " = " + Result);
        break;

      case '*':
        Result = Num1 * Num2;
        System.out.println(Num1 + " * " + Num2 + " = " + Result);
        break;

      case '/':
        Result = Num1 / Num2;
        System.out.println(Num1 + " / " + Num2 + " = " + Result);
        break;
     case '%':
        Result = Num1 % Num2;
        System.out.println(Num1 + " %" + Num2 + " = " + Result);
        break;
      default:
        System.out.println("Invalid operator!");
        break;
    }

  
  }
}
