# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Nirwan Rasyid Ridlo
<br>NIM		:	1227050105
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
<br>Untuk memenuhi tugas ujian akhir semester dengan membuat 2 program menggunakan bahasa c++. Program pertama untuk menampilkan nilai transpose dari matriks yaitu mengubah baris menjadi kolom dan sebalikanya dengan nilai baris dan kolom yang di inputkan. Program kedua untuk menampilkan bilangan yang habis dibagi 3, 5, dan 7 dengan nilai yang di inputkan pada baris dan kolom menggunakan array 2 dimensi
## Source Code
#Program 1
	
	#include <iostream>
	#include <conio.h>
	using namespace std;

	main()
	{
	int matr[20][20];
	int trans[20][20];
	int i, j, x, y;
	int jml = 0;
		cout<<" TRANSPOSE MATRIKS "<<endl;
		cout<<"=========================\n"<<endl;
		
 		cout << "Masukkan jumlah baris matriks: ";
 		cin >> x;
 		cout << "Masukkan jumlah kolom matriks: ";
  		cin >> y;

	cout<<endl;
	for (i=0; i<x; i++)
		for (j=0; j<y; j++)
		{
			cout<<"masukan elemen baris ke "<<i+1<<" kolom ke "<<j+1<<" = ";
			cin>>matr[i][j];
		}
	cout<<endl;
	cout<<"======= Elemen Matriks ======="<<endl;
	for (i=0; i<x; i++)
	{
		for (j=0; j<y; j++)
		{
			cout<<matr[i][j]<<"\t";
		}
	cout<<endl;
	}
	for (i = 0; i < x; i++)
	{
    	for (j = 0; j < y; j++)
		{
     		trans[j][i] = matr[i][j];
  	 	}
 	}
 	cout<<"======= Hasil Transpose ======="<<endl;
 	for (i=0; i<y; i++)
 	{
 		for (j=0; j<x; j++)
		{
			cout<<trans[i][j]<<"\t";
		}
	cout<<endl;	
	}
	getch();
	}

#Program 2
	
	#include <iostream>
	#include <conio.h>
	using namespace std;
	main()
	{
 	int matr[20][20];
	int trans[20][20];
	int i, j, x, y;
		cout<<"Menampilkan bilang yang habis dibagi 3,5,7 "<<endl;
		cout<<"=========================\n"<<endl;
		
 		cout << "Masukkan jumlah baris : ";
 		cin >> x;
 		cout << "Masukkan jumlah kolom : ";
  		cin >> y;

	cout<<endl;
	for (i=0; i<x; i++)
		for (j=0; j<y; j++)
		{
			cout<<"masukan elemen baris ke "<<i+1<<" kolom ke "<<j+1<<" = ";
			cin>>matr[i][j];
		}
	cout<<endl;
	cout<<"======= Nilai habis di bagi 3 ======="<<endl;
	
	for (i=0; i<x; i++)
	{
		for (j=0; j<y; j++)
		{
			if(matr[i][j]%3==0)
			{
				cout<<" "<<matr[i][j];
			}			
		}
	}
	cout<<endl;
	cout<<"======= Nilai habis di bagi 5 ======="<<endl;
	
	for (i=0; i<x; i++)
	{
		for (j=0; j<y; j++)
		{
			if(matr[i][j]%5==0)
			{
				cout<<" "<<matr[i][j];
			}			
		}
	}
	cout<<endl;
	cout<<"======= Nilai habis di bagi 7 ======="<<endl;
	
	for (i=0; i<x; i++)
	{
		for (j=0; j<y; j++)
		{
			if(matr[i][j]%7==0)
			{
				cout<<" "<<matr[i][j];
			}			
		}
	}
	cout<<endl;
	cout<<"======= Nilai habis di bagi 3,5,7 ======="<<endl;
	
	for (i=0; i<x; i++)
	{
		for (j=0; j<y; j++)
		{
			if(matr[i][j]%3==0 && matr[i][j]%5==0 && matr[i][j]%7==0)
			{
				cout<<" "<<matr[i][j];
			}			
		}
	}
	}	
## Output
<br>TRANSPOSE MATRIKS
<br>=========================

<br>Masukkan jumlah baris matriks: 2
<br>Masukkan jumlah kolom matriks: 3

<br>masukan elemen baris ke 1 kolom ke 1 = 2
<br>masukan elemen baris ke 1 kolom ke 2 = 1
<br>masukan elemen baris ke 1 kolom ke 3 = 3
<br>masukan elemen baris ke 2 kolom ke 1 = 4
<br>masukan elemen baris ke 2 kolom ke 2 = 5
<br>masukan elemen baris ke 2 kolom ke 3 = 6

<br>======= Elemen Matriks =======
<br>2       1       3
<br>4       5       6
<br>======= Hasil Transpose =======
<br>2       4
<br>1       5
<br>3       6

<br>Menampilkan bilang yang habis dibagi 3,5,7
<br>=========================

<br>Masukkan jumlah baris : 3
<br>Masukkan jumlah kolom : 3

<br>masukan elemen baris ke 1 kolom ke 1 = 28
<br>masukan elemen baris ke 1 kolom ke 2 = 21
<br>masukan elemen baris ke 1 kolom ke 3 = 35
<br>masukan elemen baris ke 2 kolom ke 1 = 70
<br>masukan elemen baris ke 2 kolom ke 2 = 105
<br>masukan elemen baris ke 2 kolom ke 3 = 67
<br>masukan elemen baris ke 3 kolom ke 1 = 88
<br>masukan elemen baris ke 3 kolom ke 2 = 25
<br>masukan elemen baris ke 3 kolom ke 3 = 18

<br>======= Nilai habis di bagi 3 =======
<br> 21 105 18
<br>======= Nilai habis di bagi 5 =======
<br> 35 70 105 25
<br>======= Nilai habis di bagi 7 =======
<br> 28 21 35 70 105
<br>======= Nilai habis di bagi 3,5,7 =======
<br> 105
