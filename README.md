# Praktikum7
## Latihan1.cpp

**Alur Algoritma**
1. Mulai program tersebut
2. Input interger fungsi (int, int)
3. Input integer a dan b dan deskripsikan a=0, dan b=1.
4. Jika nilai suku satu (b) adalah =1 dan jika nilai suku dua (a) adalah =0
5. Maka cetak rumus fungsi iteratif menggunakan for intruksikan fungsi fibionicci di awali dengan 2 dan diakhiri dengan i.
6. Deskripsikan variabel untuk mencetak fungsi selanjutnya
7. Cetak suku fibionicci menggunakan pemanggilan fungsi iteratif.

Pseudecode

    int typedatar (a, b)
    if (bill=1) return a
    if (bill=0) return b
    for (int i=2; i<=bil; i++)
    c= a+b, a=b, b=c
    end

CODE PROGRAM

    #include<iostream>

    using namespace std;

    int iteratif (int bil, int a, int b, int c)
    {
    a=, b=1;
    if (bil == 1) return b;
    if (bil == 0) return a;

    else{
    for(int i=2; i<=bil; i++){

    c = a + b;
    a = b;
    b = c;
    }
    return c;
    }
    }

    int main()
    {
    int bil, a, b, c;

    cout<<"Masukan Bilangan Deret ke-: ";
    cin>>bil;
    cout<<"\nBilangan fibonaccinya untuk "<<bil<<" adalah ";
    cout<< iteratif ( bil, a, b, c);

    return 0;
    }

Hasil

## Latihan2.cpp

**Alur Algoritma**
1. Mulai program tersebut
2. Input integer fungsi (int a, int b)
3. Jika nilai integer (b==0) return 0
4. Jika nilai (b>0) intruksikan return a + type data (a, b - 1)
5. Sebaliknya return (-a) + type data (a, b + 1)
6. Masukan variabel a,b untuk menginput nilai awal dan dibagi dengan nilai selanjutnya
7. Cetak nilai perkalian dengan memanggil fungsi rekrusif menggunakan type datanya.

Pseudecode

    Deskripsi a x b =
    1. 0, untuk b = 0
    2. a + (a x (b-1)), untuk b> 0
    3. -a + (a x (b + 1)), untuk b < 0
    4. End

CODE PROGRAM

    #include<iostream>
    using namespace std;

    int kali_rekursif(int a, int b)
    {
    if (b==0)
        return 0;
    else if (b > 0)
        return a + kali_rekursif(a, b - 1);
    else
        return (-a) + kali_rekursif(a, b + 1);
    }

    main()
    {
    int a, b;
    cout << "Masukan Bilangan : ";
    cin >> a;
    cout << "Dikali Dengan : ";
    cin >> b;
    cout << " AxB == " << kali_rekursif(a, b) << endl;
    }

Hasil

## Latihan3.cpp

**Alur Algoritma**
1. Mulai program tersebut
2. Input menggunakan intruksi void dan menggunakan pointer untuk menetapkan void typedata (char *s)
3. Jika nilai s!=0--> menggunakan Pointer(*) maka masukan intruksi membalik (&s[1])
4. Masukan char untuk intruksi kata yang ingin kita ubah dan intruksi balik
5. Cetak pembalikan kata dengan memanggil fungsi rekrusif menggunakan type datanya

Pseudecode

    #include
    #include
    void balik(char *k){
    if(*k!="){
    balik(&k[1]);
    cout<
    }
    }main(){
    char *kata="....";-->//untuk masukan kata
    balik(kata);
    cout<
    return 0;

CODE PROGRAM

    #include<iostream>
    #include<string.h>

    using namespace std;
    void balik(char *s)
    { if (*s != '\0'){
    balik(&s[1]);
    cout << s[0];
    }
    }
    int main()
    {
    char* kata = (char*) "Inka";
    balik(kata) ; cout << endl;
    return 0;
    }

Hasil
