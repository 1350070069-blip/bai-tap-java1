# bai-tap-java1
// De bai 1: Tinh tong, hieu, tich, thuong cua hai so nhap tu ban phim

public class Bai1 {
    public static void main(String[] args) {

        int a = 10;
        int b = 20;

        int tong = a + b;
        int hieu = a - b;
        int tich = a * b;
        double thuong = (double) a / b;

        System.out.println("Tong = " + tong);
        System.out.println("Hieu = " + hieu);
        System.out.println("Tich = " + tich);
        System.out.println("Thuong = " + thuong);
    }
}

// De bai 2: Nhap vao 2 canh a, b. Tinh chu vi va dien tich hinh chu nhat

public class Bai2 {
    public static void main(String[] args) {

        int a = 10;
        int b = 20;

        int chuVi = 2 * (a + b);
        int dienTich = a * b;

        System.out.println("Chu vi = " + chuVi);
        System.out.println("Dien tich = " + dienTich);
    }
}

// De bai 3: Viet chuong trinh xep loai hoc luc

public class Bai3 {
    public static void main(String[] args) {

        int diem = 8;

        if (diem >= 0 && diem <= 4) {
            System.out.println("Yeu");
        } else if (diem <= 6) {
            System.out.println("Trung binh");
        } else if (diem <= 8) {
            System.out.println("Kha");
        } else {
            System.out.println("Gioi");
        }
    }
}

// De bai 4: Nhap vao so n, kiem tra xem n co phai so nguyen to khong

public class Bai4 {
    public static void main(String[] args) {

        int n = 7;
        boolean laSoNguyenTo = true;

        if (n < 2) {
            laSoNguyenTo = false;
        } else {
            for (int i = 2; i <= n / 2; i++) {
                if (n % i == 0) {
                    laSoNguyenTo = false;
                    break;
                }
            }
        }

        if (laSoNguyenTo) {
            System.out.println(n + " la so nguyen to");
        } else {
            System.out.println(n + " khong phai la so nguyen to");
        }
    }
}

// De bai 5: Su dung cau truc while tinh tong cac so le tu 1 den n

public class Bai5 {
    public static void main(String[] args) {

        int n = 10;
        int s = 0;
        int i = 1;

        while (i <= n) {
            s += i;
            i += 2;
        }

        System.out.println("Tong cac so le = " + s);
    }
}

// De bai 6: Tinh tong cac so tu nhien tu 1 den n su dung vong lap for


public class Bai6 {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        System.out.print("Nhap n: ");
        int n = sc.nextInt();

        int tong = 0;

        for (int i = 1; i <= n; i++) {
            tong += i;
        }

        System.out.println("Tong = " + tong);
    }
}

// De bai 7: Tinh tong cac so nguyen duong nho hon 12

public class Bai7 {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int tong = 0;

        for (int i = 1; i < 12; i++) {
            tong += i;
        }

        System.out.println("Tong = " + tong);
    }
}

// De bai 8: Tinh tong cac so chan tu 1 den n

public class Bai8 {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        System.out.print("Nhap n: ");
        int n = sc.nextInt();

        int tong = 0;

        for (int i = 2; i <= n; i += 2) {
            tong += i;
        }

        System.out.println("Tong cac so chan = " + tong);
    }
}
