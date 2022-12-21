  # Ujian Akhir Semester 
  <br> Mata Kuliah 	: Dasar pemerograman
  <br> Nama		      : Viqriza Ahmad Vahira
  <br> NIM		      :	1227050132
  <br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

  ## Deskripsi Umum
  Ini Adalah Tugas UAS (Ulangan Tengah Semester) Yang Menjelaskan tentang:
  1.meng inputkan nilai matriks lalu mengubahnya baris menjadi kolom kolom menjadi baris
  2.Array 2 dimensi lalu ci cekbilangan yang bisa di bagi 3, 5, Dan 7

    ## Source Code
    #include <iostream>

    using namespace std;

    int main(){
      cout<<"====================================================================================="<<endl;
      cout<<"Nama   : Viqriza Ahmad Vahira                                                        "<<endl;
      cout<<"NIM    : 1227050132                                                                  "<<endl;
      cout<<"Matkul : Dasprog UAS (Ulangan Akhir Semester)                                        "<<endl;
      cout<<"====================================================================================="<<endl;
      cout<< "                                                                                    "<<endl;
      cout<<"----------------------------------------Bissmilah------------------------------------"<<endl;
      cout<<"                                                                                     "<<endl;

      int v, p, o, x, matriks[10][10], transpose[10][10];

      cout << "Inputkan jumlah baris matriks: ";
      cin >> o;
      cout << "Inputkan jumlah kolom matriks: ";
      cin >> x;

      cout << "Inputkan elemen matriks\n";
      for (v = 0; v < o; v++){
        for (p = 0; p < x; p++){
           cout <<"("<<v<<","<<p<<") : ";
          cin  >> matriks[v][p];
        }
      }
      cout << endl;

      for (v = 0; v < o; v++){
        for (p = 0; p < x; p++){
          cout << matriks[v][p] << "\t";
        }
        cout << endl;
      }
      cout << endl;

      for (v = 0; v < o; v++){
        for (p = 0; p < x; p++){
          transpose[p][v] = matriks[v][p];
        }
      }

      cout << "Hasil Transpose Matriks: \n";
      for (v = 0; v < x; v++){
        for (p = 0; p < o; p++){
          cout << transpose[v][p] << "\t";
        }
        cout << endl;
      }
      cout<<endl<<endl;
      cout<<" No 2 Program mengecek nilai yang habis dibagi 3,5, dan 7 "<<endl;
      int data[10][10];
      cout << "Masukkan jumlah baris : ";
      cin >> o;
      cout << "Masukkan jumlah kolom : ";
      cin >> x;
      cout<<endl;
      cout << "Masukkan elemen array\n";
      for (v = 0; v < o; v++){
      for (p = 0; p < x; p++) {
           cout <<"Baris ke-"<<v+1<<", Kolom ke-"<<p+1<<" : ";
             cin  >> data[v][p];
        }
      }
      cout << endl;
      cout<<" Nilai yang di input : "<<endl;
      for (v = 0; v < o; v++){
        for (p = 0; p < x; p++){
          cout << data[v][p] << "\t";
        }
        cout << endl;
      }
      cout << endl;

      bool kondisi= true;
      cout<<" Nilai yang habis dibagi 3 5 dan 7 : "<<endl;
      for (int v=0; v<o; v++ ) {
        for (int p=0; p<x; p++) {
          if (data[v][p]%3==0 && data[v][p]%5==0 && data[v][p]%7==0) {
            cout<<data[v][p];
            cout<<endl;
            kondisi= false;
          }

        }
      }

      if (kondisi) {
    cout<<" tidak ada bilangan yang habis dibagi 3 5 dan 7 :"<<endl;
     }
     return 0;


    }


    ## Output
    Inputkan jumlah baris matriks: 2
    Inputkan jumlah kolom matriks: 2
    Inputkan elemen matriks
    (0,0) : 1
    (0,1) : 3
    (1,0) : 4
    (1,1) : 7

    1       3
    4       7

    Hasil Transpose Matriks:
    1       4
    3       7
    
    
     No 2 Program mengecek nilai yang habis dibagi 3,5, dan 7
    Masukkan jumlah baris : 2
    Masukkan jumlah kolom : 2

    Masukkan elemen array
    Baris ke-1, Kolom ke-1 : 2
    Baris ke-1, Kolom ke-2 : 105
    Baris ke-2, Kolom ke-1 : 4
    Baris ke-2, Kolom ke-2 : 210

     Nilai yang di input :
    2       105
    4       210

     Nilai yang habis dibagi 3 5 dan 7 :
    105
    210
