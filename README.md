# artik
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);
        int year;
        System.out.print(" Lütfen kontrol etmek istediğiniz yılı giriniz: ");
        year = input.nextInt();

        if (year % 4 == 0 || year % 100 == 0) {
            if (year % 100 == 0 && year % 400 != 0) {
                System.out.print(" Girdiğiniz yıl, artık yıl değildir. ");
            }else if (year % 100 == 0 && year % 400 == 0) {
                System.out.print(" Girdiğiniz yıl, artık yıldır. ");
            }else {
                System.out.print(" Girdiğiniz yıl, artık yıldır. ");
            }
        }else {
            System.out.print(" Girdiğiniz yıl, artık yıl değildir.");
        }
    }
}
