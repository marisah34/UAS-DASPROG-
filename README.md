# UJIAN AKHIR SEMESTER 
<br>Mata Kuliah : Dasar Pemrograman 
<br> Nama : Marisah Lofiana 
<br> NIM : 1227050068
<br>Jurusan : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/)

## Deskripsi umum 
Matriks merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks.

## source code 

        #include <iostream>
        using namespace std;
        int main(){
          int i, j, m, n, matriks[50][50], transpose[50][50];
          cout << "Masukkan jumlah baris : ";
          cin >> m;
          cout << "Masukkan jumlah kolom : ";
          cin >> n;
          cout << "Masukkan elemen matriks\n";
          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              cin  >> matriks[i][j];
            }
          }
          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              transpose[j][i] = matriks[i][j];
            }
          }
          cout << "\nHasil Transpose Matriks: \n";
          for (i = 0; i < n; i++){
            for (j = 0; j < m; j++){
              cout << transpose[i][j] << "\t";
            }
            cout << endl;
          }
          return 0;
        }
        
        
        
        #include <iostream>
        #include <iomanip>
        using namespace std;
        int main(){
            int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

            cout<<"Input jumlah baris: "; cin>>jumlahBaris;
            cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
            cout << endl;

            for(i = 0; i < jumlahBaris; i++){
                for(j = 0; j < jumlahKolom; j++){
                    cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
                    cin >> arr[i][j];
                }
                cout << endl;
            }

            cout << "Hasil matriks: " << endl;

            for(i = 0; i < jumlahBaris ; i++){
            for(j = 0; j < jumlahKolom; j++){
                cout << setw(3) << arr[i][j] << " ";
            }
            cout << endl;
            }

            cout << "\nHasil habis di bagi 3 5 7 adalah : " << endl;

            for(i = 0; i < jumlahBaris ; i++){
            for(j = 0; j < jumlahKolom; j++){
                if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
                cout << setw(3) << arr[i][j] << " ";
                }
            }
            cout << endl;
            }


            cout << endl;
            return 0;
        }
        
        



## output 
  
Masukkan jumlah baris : 3
Masukkan jumlah kolom : 3
Masukkan elemen matriks
2 3 4
5 6 7
8 9 1

Hasil Transpose Matriks:
2       5       8
3       6       9
4       7       1

--------------------------------
Process exited after 13.08 seconds with return value 0
Press any key to continue . . .


Input jumlah baris: 3
Input jumlah kolom: 3

Baris 1, kolom 1 = 1
Baris 1, kolom 2 = 2
Baris 1, kolom 3 = 3

Baris 2, kolom 1 = 4
Baris 2, kolom 2 = 5
Baris 2, kolom 3 = 6

Baris 3, kolom 1 = 7
Baris 3, kolom 2 = 8
Baris 3, kolom 3 = 9

Hasil matriks:
  1   2   3
  4   5   6
  7   8   9

Hasil habis di bagi 3 5 7 adalah :
  3
  5   6
  7   9


--------------------------------
Process exited after 16.51 seconds with return value 0
Press any key to continue . . .
  
  
  
