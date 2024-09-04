import java.util.Scanner;

public class netPay {
    static String name;
    static double hoursWorked;
    static double RATE_PER_HOUR;
    static double SSS;
    static double TAX;
    static double PIGIBIG;
    static double totalDeduction;

    public static void inp() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("WHAT IS YOUR NAME? ");
        name = scanner.nextLine();
        System.out.print("WHAT IS THE NO OF THE HOURS WORKED? ");
        hoursWorked = scanner.nextDouble();
        System.out.print("WHAT IS THE RATE PER HOUR? ");
        RATE_PER_HOUR = scanner.nextDouble();
        System.out.print("WHAT IS THE SSS CONTRIBUTION? ");
        SSS = scanner.nextDouble();
        System.out.print("WHAT IS THE TAX RATE? ");
        TAX = scanner.nextDouble();
        System.out.print("WHAT IS THE PIGIBIG CONTRIBUTION? ");
        PIGIBIG = scanner.nextDouble();
    }
    public static double computeGrossPay(double noOfHourWork, double RATE_PER_HOUR) {
        return noOfHourWork * RATE_PER_HOUR;
    }

    public static double computeDeduction(double grossPay) {
        totalDeduction = grossPay * (SSS + TAX + PIGIBIG) / 100;
        return totalDeduction;
    }

    public static double computeNetPay(double grossPay, double deduction) {
        return grossPay - deduction;
    }

    public static void displayResult() {
        double grossPay = computeGrossPay(hoursWorked, RATE_PER_HOUR);
        double deduction = computeDeduction(grossPay);
        double netPay = computeNetPay(grossPay, deduction);

        System.out.println("Employee Name: " + name);
        System.out.println("Gross Pay: " + grossPay);
        System.out.println("Total Deduction: " + deduction);
        System.out.println("Net Pay: " + netPay);
    }
}
