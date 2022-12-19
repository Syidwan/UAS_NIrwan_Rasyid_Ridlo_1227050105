# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Nirwan Rasyid Ridlo
<br>NIM		:	1227050105
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
<br>Untuk memenuhi tugas ujian akhir semsester dengan membuat 2 program menggunakan bahas c++. Program pertama untuk menampilkan nilai transpose dari matriks uyaitu mengubah baris menjadi kolom dan sebalikanya dengan nilai yang di inputkan. Program kedua untuk menampilkan bilangan yang habis dibagi 3,5,7

## Source Code
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
## Output
