# Decimal-to-Binary
it will change decimal no. to binary no.
import java.util.Scanner;

public class decimaltobinary {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int decimal_no = sc.nextInt();
        int ans = 0;
        int pw = 1;
        while (decimal_no>0){
            int parity = decimal_no % 2;
            ans += (parity*pw);
            pw*=10;
            decimal_no /= 2;
        }
        System.out.println(ans);
    }
}
