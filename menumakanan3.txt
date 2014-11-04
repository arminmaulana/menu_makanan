import javax.swing.JOptionPane;

class MenuMakanan3
{
 public static void main(String[] args) 
 {
  String pilihMakananString;
  String pilihNasiString;
        String pilihIkanString;
  String pilihSayurString;
  String pilihAnekaString;

  int pilihMakanan;
  int pilihNasi;
  int pilihIkan;
  int pilihSayur;
  int pilihAneka;

  do
  {
            pilihMakananString = JOptionPane.showInputDialog ("Menu Makanan : \n1. Nasi \n2. Ikan \n3. Sayur");
      pilihMakanan = Integer.parseInt (pilihMakananString);
  }
  while (pilihMakanan > 3 || pilihMakanan < 1);

  switch (pilihMakanan)
  {
  case 1:
   do
   {
                pilihNasiString = JOptionPane.showInputDialog ("Menu Nasi : \n1. Nasi Putih \n2. Nasi Uduk  \n3. Nasi Goreng Spesial");
          pilihNasi = Integer.parseInt (pilihNasiString);
   }
   while (pilihNasi > 3 || pilihNasi < 1);
          switch (pilihNasi)
          {
          case 1: JOptionPane.showMessageDialog (null, "Anda Memilih Nasi Putih");
    break;
          case 2: JOptionPane.showMessageDialog (null, "Anda Memilih Nasi Uduk");
    break;
    case 3: JOptionPane.showMessageDialog (null, "Anda Memilih Nasi Goreng Spesial");
    break;
          }
  break;
        case 2: 
   do
   {
                pilihIkanString = JOptionPane.showInputDialog ("Menu Ikan : \n1. Ikan Tongkol Sambal \n2. Kambing Gulai \n3. Aneka Penyet");
          pilihIkan = Integer.parseInt (pilihIkanString);
   }
   while (pilihIkan > 3 || pilihIkan < 1);
    switch (pilihIkan)
    {
    case 1: JOptionPane.showMessageDialog (null, "Anda Memilih Ikan Tongkol Sambal");
    break;
    case 2: JOptionPane.showMessageDialog (null, "Anda Memilih Kambing Gulai");
    break;
    case 3: 
     do
     {
     pilihAnekaString = JOptionPane.showInputDialog ("Menu Aneka Penyet : \n1. Ayam Penyet Spesial \n2. Ayam Penyet Biasa \n3. Bebek Penyet \n4. Burung Penyet");
        pilihAneka = Integer.parseInt(pilihAnekaString);
     }
     while (pilihAneka > 4 || pilihAneka < 1);
     switch (pilihAneka)
     {
     case 1: JOptionPane.showMessageDialog (null, "Anda Memilih Ayam Penyet Spesial");
     break;
     case 2: JOptionPane.showMessageDialog (null, "Anda Memilih Ayam Penyet Biasa");
     break;
     case 3: JOptionPane.showMessageDialog (null, "Anda Memilih Bebek Penyet");
     break;
     case 4: JOptionPane.showMessageDialog (null, "Anda Memilih Burung Penyet");
     break;
     }
    break;
    }
  break;
  case 3: 
   do
   {
       pilihSayurString = JOptionPane.showInputDialog ("Menu Sayur : \n1. Sayur Gulai \n2. Sayur Daun Ubi Tumbuk \n3. Sayur Campur");
          pilihSayur = Integer.parseInt (pilihSayurString);
   }
   while (pilihSayur > 3 || pilihSayur < 1);
    switch (pilihSayur)
    {
    case 1: JOptionPane.showMessageDialog (null, "Anda Memilih Sayur Gulai");
    break;
    case 2: JOptionPane.showMessageDialog (null, "Anda Memilih Sayur Daun Ubi Tumbuk");
    break;
    case 3: JOptionPane.showMessageDialog (null, "Anda Memilih Sayur Campur");
    break;
    }
  }
  JOptionPane.showMessageDialog (null, "Silahkan Ditunggu, Pesanan Segera Diantar." + "\nTerima Kasih." + "\nSelamat Menikmati. ^_^");
  System.out.println ("Selesai !!!!!!!!");
 }
}