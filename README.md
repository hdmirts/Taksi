## Km Cinsinden Taksimetre Tutar Hesaplama:

Taksimetre km başına 2.20 tl tutuyor.
Açılış ücreti = 10 tl.
Min. ödeme tutarı = 20 tl.
20 Tl'nin altındaki tutarda da ödeme 20 tl alınır.;

```java
import java.util.Scanner;
public class taksi {
    public static void main(String[] args) {
        
        int km;
        double perKm = 2.20, total;
        Scanner input = new Scanner(System.in);
        System.out.print("Mesafeyi Km Cinsinden Giriniz :");
        km = input.nextInt();
        total = (km * perKm) + 10;
    

        total = (total < 20) ? 20 : total; //min tutar 20 tl.Tutar 20den düşükse 20'yi, değilse (:) o değeri versin
        System.out.println("Toplam tutar :" + total);

    }
    
}

```



***Şu şekilde de yapılabilir:***



```java
import java.util.Scanner;
public class taksi {
    public static void main(String[] args) {
        
        int km;
        double perKm = 2.20, total, startPrice = 10;
        Scanner input = new Scanner(System.in);
        System.out.print("Mesafeyi Km Cinsinden Giriniz :");
        km = input.nextInt();
        total = (km * perKm) + startPrice;
          total = (total < 20) ? 20 : total;
        System.out.println("Toplam tutar :" + total);

    }
    
}

```

