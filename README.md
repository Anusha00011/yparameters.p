# yparameters.p
y parameters in Java programming 
import java.util.Scanner;

public class YParameters {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        double Y11, Y12, Y21, Y22;
        double V1, V2, I1, I2;

        System.out.print("Enter Y11: ");
        Y11 = sc.nextDouble();

        System.out.print("Enter Y12: ");
        Y12 = sc.nextDouble();

        System.out.print("Enter Y21: ");
        Y21 = sc.nextDouble();

        System.out.print("Enter Y22: ");
        Y22 = sc.nextDouble();

        System.out.print("Enter V1: ");
        V1 = sc.nextDouble();

        System.out.print("Enter V2: ");
        V2 = sc.nextDouble();

        // Calculate currents
        I1 = (Y11 * V1) + (Y12 * V2);
        I2 = (Y21 * V1) + (Y22 * V2);

        System.out.printf("\nI1 = %.2f A", I1);
        System.out.printf("\nI2 = %.2f A", I2);

        sc.close();
    }
}