TEMEL VERİ TİPLERİ 

double sayi1= 12.5;
boolean dogruMu=false;
char karakter= 'a';
HELLO WORLD

public static void main(String[] args) {
        System.out.println("Merhaba Java");
        System.out.println("Merhaba Java2");
    }
}


DEĞİŞKENLER

 public static void main(String[] args) {
        int ogrenciSayisi = 12;
        String mesaj = "Öğrenci sayısı: ";
        System.out.println(mesaj + ogrenciSayisi);
        System.out.println(mesaj + ogrenciSayisi);
        System.out.println("öğrenci sayım:" + ogrenciSayisi);
        System.out.println("öğrenci sayım:" + ogrenciSayisi);
        System.out.println("öğrenci sayım:" + ogrenciSayisi);
    }
}


DATATYPES

public class Main {
    public static void main(String[] args) {

        double sayi1= 12.5;
        boolean dogruMu=false;
        char karakter= 'a';

    }
}






IF BLOĞU

{
    public static void main(String[] args) {
        int sayi =2;
        if (sayi < 20) {
            System.out.println("sayı 20den küçüktür");

        }
        else if (sayi==20){
            System.out.println("sayı 20ye eşittir");
        } else {
            System.out.println("sayı 20den büyüktür");

        }
    }
}

DEMO1

  public static void main(String[] args) {
        int sayi1 =20;
        int sayi2 =25;
        int sayi3 =2;
        int enBuyuk = sayi1;

        if(enBuyuk<sayi2) {
            enBuyuk =sayi2;
        }
        if (enBuyuk<sayi3) {
            enBuyuk=sayi3;
        }
        System.out.println("En Büyük = "+ enBuyuk);
    }
}



SWITCH

public class Main {
    public static void main(String[] args) {
       char grade = 'D';
       switch(grade) {
           case 'A':
              System.out.println("mükemmel: Geçtiniz");
              break;
           case 'B':
               System.out.println("Çok güzel: Geçtiniz");
               break;
           case 'C':
               System.out.println("İyi: Geçtiniz");
               break;
           case 'D':
               System.out.println("Fena Değil: Geçtiniz");
               break;
           case 'F':
               System.out.println("Maalesef: Kaldınız");
               break;
           default:
               System.out.println("GEÇERSİZ");

       }
    }
}


FOR, WHİLE, DO -WHİLE DÖNGÜSÜ

public class Main {
    public static void main(String[] args) {
        for(int i=2;i<10;i+=2)

        {
            System.out.println(i);
        }
        System.out.println("FOR döngü bitti");

        int i=1;
        while(i<10) {
            System.out.println(i);
            i++;

        }
        System.out.println("While döngü bitti");

        int j=100;
        do {
            System.out.println(j);
            j+=2;
        }
        while(j<10);
        System.out.println("do - while döngü bitti");

    }
}



DİZİLER

public class Main {
    public static void main(String[] args) {
        String ogrenci1 ="Engin";
        String ogrenci2 ="Derin";
        String ogrenci3 ="Salih";
        String ogrenci4 ="Ahmet";

        System.out.println(ogrenci1);
        System.out.println(ogrenci2);
        System.out.println(ogrenci3);
        System.out.println(ogrenci4);

        System.out.println("----------");

        String[] ogrenciler = new String[4];
        ogrenciler[0]="Engin";
        ogrenciler[1]="Derin";
        ogrenciler[2]="Salih";
        ogrenciler[3]="Ahmet";


        for(int i=0;i<ogrenciler.length; i++)
        {
            System.out.println(ogrenciler[i]);
        }


    }
}


DEMO2

public class Main {
    public static void main(String[] args) {

        double[] myList = {1.2, 1.3, 4.3, 5.6};
        double total = 0;
        double max= myList[0];
        for (double number : myList) {
            if(max<number){
                max=number;
            }
            total = total + number;
            {
                System.out.println(number);
            }
            System.out.println("Toplam =" + total);
            System.out.println("En Büyük  =" + max);

        }
    }
}

Çok boyutlu diziler

public class Main {
    public static void main(String[] args) {
        String[][] sehirler = new String[3][3];
        sehirler[0][0] = "istanbul";
        sehirler[0][1] = "Bursa";
        sehirler[0][2] = "Bilecik";
        sehirler[1][0] = "Konya";
        sehirler[1][1] = "Ankara";
        sehirler[1][2] = "Kayseri";
        sehirler[2][0] = "Diyarbakır";
        sehirler[2][1] = "Şanlıurfa";
        sehirler[2][2] = "Antep";

        for (int i = 0; i <= 2; i++) {
            System.out.println("--------------");

            for (int j = 0; j <= 2; j++) {
                System.out.println(sehirler[i][j]);
            }

        }
    }
}



STRİNG 


public class Main {
    public static void main(String[] args) {
        String mesaj = "    bugün hava  Çok Güzel";
        System.out.println(mesaj);

        System.out.println("Eleman Sayısı :" +mesaj.length());
        System.out.println("5. Eleman  :" +mesaj.charAt(4));
        System.out.println(mesaj.concat(" YAŞAIN!"));
        System.out.println(mesaj.startsWith("A"));
        System.out.println(mesaj.endsWith("."));
        char[] karakterler = new char[5];
        mesaj.getChars(0,5, karakterler,0);
        System.out.println(karakterler);
        System.out.println(mesaj.indexOf("a"));


        System.out.println(mesaj.replace(' ', '-'));
        System.out.println(mesaj.substring(2));

        for (String kelime : mesaj.split(" ")) {
            System.out.println(kelime);
        }

        System.out.println(mesaj.toLowerCase());


    }
}


ASAL SAYI

public class Main {
    public static void main(String[] args) {
        int number =1;
        int remainder = number % 2;
        System.out.println(remainder);
        boolean inPrime=true;

        if (number<2){
            System.out.println("GEÇERSİZ");
        }

        for (int i=2; i<number; i++)
        {
            if(number % i ==0){
                inPrime=false;
            }

        }
        if (inPrime){
            System.out.println("Sayınız asaldır");
        } else{
            System.out.println("sayınız asal değildir");
        }
    }


KALIN_İNCE SESLİ HARFLER

public class Main {
    public static void main(String[] args) {
        char harf='E';
        switch (harf) {
            case 'A':
            case 'I':
            case 'o':
            case 'U':
                System.out.println("kalın sesli harf ");
                break;
            default:
                System.out.println("Kalın seesiz HArf");
        }
    }
}

MÜKEMMEL SAYI 

public class Main {
    public static void main (String[] args) {
        int number =28;
        int total=0;
        for(int i=0; i<number; i++){
            if(number% i==0) {
                total=total+ i;
            }
        }
if (total==number) {
    System.out.println("Mükemmel sayıdır");
} else {
    System.out.println("Değildir");
}
    }
}


ARKADAŞ SAYILAR

public class Main {
    public static void main(String[] args) {
       int sayi1=220;
       int sayi2=224;
       int toplam1=0;
        int toplam2=0;

        for (int i=1; i<sayi1;i++){
            if (sayi1%i==0){
                toplam1= toplam1+i;
            }
        }
        for (int i=1; i<sayi2;i++){
            if (sayi2%i==0){
                toplam2= toplam2+i;

    }
        }
        if (sayi1==toplam2 && sayi2 ==toplam1){
            System.out.println("bu iki sayı arkadaş");
        }
        else {
            System.out.println("arkadaş değildir");
        }
    }
}



SAYI BULMA

public class Main {
    public static void main(String[] args) {
        int[] sayilar = new int[]{1,2,5,7,9,0};
        int aranacak=5;
        boolean varMi=false;

        for (int sayi: sayilar){
            if (sayi==aranacak){
                varMi= true;
                break;
            }
        }
        if (varMi){
            System.out.println("sayı mevcuttur.");
        }
        else {
            System.out.println("sayı mevcut değildir.");
        }
    }
}
