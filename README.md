# GreatestOr
import java.util.*;

public class Greatest {
	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);
		int input1 = in.nextInt();
		int input2 = in.nextInt();
		Greatest gr = new Greatest();
		gr.printGcd(input1, input2);
	}

	public void printGcd(int input1, int input2) {
		if (input1 > 0 && input2 > 0) {

			System.out.println("greatest common divisor " + reGcd(input1, input2));
		} else {
			System.err.println("Please check input > 0");
		}
	}

	public int reGcd(int input1, int input2) {
		if (input2 > 0) {
			return reGcd(input2, input1 % input2);
		} else {
			return input1;
		}

	}   
}

   
   
   
   
   
   
   
   
   
   
   

    
    
