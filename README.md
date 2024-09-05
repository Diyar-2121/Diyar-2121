using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace hesap_makinesi_basit_kodlama
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Lütfen bir sayı giriniz:");
            int a = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Lütfen ikinci sayıyı giriniz");
            int b = Convert.ToInt32(Console.ReadLine());
            int sayi1, sayi2, sayi3, sayi4;
            Console.WriteLine("istediğiniz işlemi seçin lütfen");
            Console.WriteLine("Toplama işlemi için : 'T' tuşuna basın.");
            Console.WriteLine("Çıkarma işlemi için : 'Ç' tuşuna basın.");
            Console.WriteLine("Çarpma işlemi için :'X' tuşuna basın.");
            Console.WriteLine("Bölme işlemi için : 'B' tuşuna basın.");
            string islem = Console.ReadLine();
            sayi1 = a + b;
            sayi2 = a - b;
            sayi3 = a * b;
            sayi4 = a / b;
            if (islem == "T")

            {
                Console.WriteLine("İki sayının toplamı = " + sayi1);
                Console.WriteLine("Yeni bir işlem yapmak için lütfen programı yeniden başlatın");
            }
            else if (islem == "Ç")
            {
                Console.WriteLine("İki sayının çıkarma sonucu = " + sayi2);
                Console.WriteLine("Yeni bir işlem yapmak için lütfen programı yeniden başlatın");
            }
            else if (islem == "X")
            {
                Console.WriteLine("İki sayının çarpım sonucu = " + sayi3);
                Console.WriteLine("Yeni bir işlem yapmak için lütfen programı yeniden başlatın");
            }
            else if (islem == "B")
            {
                Console.WriteLine("İki sayının bölümünün sonucu = " + sayi4);
                Console.WriteLine("Yeni bir işlem yapmak için lütfen programı yeniden başlatın");
            }
            else
            {
                Console.WriteLine("Lütfen programı yeniden başlatıp yukarıdaki harflerden birini seçerek işleme devam ediniz !!!");
            }
            Console.ReadLine();
        }
    }
}

