import java.util.Scanner;

public class kal {
    public static void main(String[] args) {
        Scanner cal = new Scanner(System.in);
        int [] angka = new int[4];
        int pilihan, total;

        System.out.println("Pilihlah Antara:");
        System.out.println("1. Penjumlahan(+)");
        System.out.println("2. Pengurangan(-)");
        System.out.print("Masukan Pilihan: ");
        pilihan = cal.nextInt();

        if(pilihan == 1){
            for(int i=0; i<4; i++){
                System.out.print("Masukan Angka Ke-"+(i+1)+": ");
                angka[i] = cal.nextInt();
            }
            total = angka[0] + angka[1] + angka[2] + angka[3];
            System.out.println("Hasil Penjumlahan: "+total);
        }else if(pilihan == 2){
            for(int i=0; i<4; i++){
                System.out.print("Masukan Angka Ke-"+(i+1)+": ");
                angka[i] = cal.nextInt();
            }
            total = angka[0] - angka[1] - angka[2] - angka[3];
            System.out.println("Hasil Pengurangan: "+total);
            
        }else{
            System.out.println("Invalid Option");
        }
        
    
    }

}
