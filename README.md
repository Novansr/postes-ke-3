# postes-ke-3
Diskon cafe dan program akun sederhana

Nomor 1

def total():
    print ("1. es teh")
    print ("2. teh hangat")
    print ("3. jus jeruk")
    print ("4. es buah")
    print ("5. air putih")
    print ("6. kopi hitam")
    print ("7. kopi susu")
    print ("8. bakso")
    print ("9. nasi goreng")
    print ("10. mie goreng")
    print ("11. mie ayam")
    print ("12. ayam geprek")
    print ("13. ayam goreng")
pilihan="Ya"
while pilihan=="Ya":
    print('''
===================================
Selamat Datang di
Toko Serba Murah
Dapat Diskon Jika :
Membeli 3 minuman = 10 %
Membeli 2 makanan = 25 %
Membayar dengan E-money = 5 %
Hari Weekend = 5 %
Hari Weekdays = 10 %
===================================''')
    total()
    menu = int(input("pilih barang yang diinginkan: "))
    if menu == 1 :
        print("es teh 3000")
        menu = 3000
    elif menu == 2 :
        print ("teh hangat 3000")
        menu = 3000
    elif menu == 3 : 
        print ("jus jeruk 4000")
        menu = 4000
    elif menu == 4 :
        print ("es buah 8000")
        menu == 8000
    elif menu == 5 :
        print ("air putih 2000")
        menu == 2000
    elif menu == 6 :
        print ("kopi hitam 8000")
        menu == 8000
    elif menu == 7 :
        print ("kopi susu 8000")
        menu == 8000
    elif menu == 8 :
        print ("bakso 10000")
        menu == 10000
    elif menu == 9 :
        print ("nasi goreng 12000")
        menu == 12000
    elif menu == 10 :
        print ("mie goreng 12000")
        menu == 12000
    elif menu == 11 :
        print ("mie ayam 12000")
        menu == 12000
    elif menu == 12 :
        print ("ayam geprek 15000")
        menu == 15000
    elif menu == 13 :
        print ("ayam goreng 10000")
        menu == 10000
    Jumlah = int(input("masukan jumlah barang yang dibeli: "))
    Total = menu*Jumlah
    pembelian = input('masukkan total pembelian: ')
    if pembelian == '3 minuman':
        Total=int(Total-0.01*Total)
        print('-Diskon 10 %-')
    elif pembelian == '2 makanan':
        Total=int(Total-0.005*Total)
        print('-Diskon 5 %-')
    pembayaran = input('masukan metode pembayaran: ')
    if pembayaran == 'E-money':
        Total=int(Total-0.005*Total)
        print('-Diskon 5 %-')
    else:
        print('Maaf,tidak dapat diskon')
    Hari = input('masukan hari pembelian: ')
    if Hari == 'weekend':
        Total=int(Total-0.005*Total)
        print('-Diskon 5 %-')
    elif Hari == 'weekdays':
        Total=int(Total-0.01*Total)
        print('-Diskon 10 %-')
    else:
        print('Maaf,tidak dapat diskon')
        print("Total Harga = ", "Rp.",Total)
    Bayar=int(input("Jumlah Nominal Uang = Rp. ", ))
    Kembalian= (Bayar-Total)
    print("Uang Kembalian = ", "Rp.",Kembalian)
    lagi=True
    while lagi==True:
        pilihan=input("Apakah anda ingin Membeli lagi Ya/Tidak= ")
        if pilihan=="Tidak":
            print('Terima Kasih Telah berbelanja di toko serba Murah')
            lagi=False
        elif pilihan=="Ya":
            print("Silahkan Memilih Kembali Menu yang tersedia")
            lagi=False
        else:
            print("Anda salah memasukkan pilihan Ya/Tidak")
            lagi=True

No2

int main(){
   char username[5]= "irma", pass[12]= "risma";
   char usr[5], pas[12];
   int status = 0, salah = 0;

   while(status < 3){
      printf("Masukkan Username : ");
      gets(usr);
      printf("Masukkan Password : ");
      gets(pas);

      if(strcmp(username, pass)==0 && strcmp (pass, pass)== 0){
         printf("Akses diterima. Selamat Datang\n");
         break;
      }else{
         printf("Username dan Password tidak match\n");
         salah++;
         if(salah == 3){
            printf("Akses ditolak\n");
         }
      }
      status++;
   }

   system("pause");
   return 0;
}
