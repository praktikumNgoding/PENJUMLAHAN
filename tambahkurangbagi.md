#include <iostream>
#include <math.h>

using namespace std ;

class h{
	public:
		static void penjumlahan(int x,int y){
			cout<<"penjumlahan :"<<x+y<<endl;
      }
		
    static void pengurangan(int x,int y){
			cout<<"pengurangan :"<<x-y<<endl;
      }
		
    void perkalian (int x,int y){
			cout<<"perkalian :"<<x*y<<endl;
      }
		
    void pembagian (double x,double y){
			cout<<"pembagian :"<<x/y<<endl;}
		
    void sederhana(int x,int y){
			int k=(x<y)?x:y;
			int q=1;
			while(q==1){
			if(x%k==0&&y%k==0){
			x=x/k;
			y=y/k;
			cout<<"penyederhanaan :"<<x<<"/"<<y<<endl;
			q=0;
		}
    else {
			k--;}}}};
		
    int main(){
			cout<<"\t\t\t\tSELAMAT DATANG DI PERHITUNGAN"<<endl;
			int x,y ;
			h nonstatic;
			cout<<"masukkan nilai x =";
			cin>>x;
			cout<<"masukkan nilai y =";
			cin>>y;
			cout<<endl;
			h::penjumlahan(x,y);
			h::pengurangan(x,y);
			nonstatic.perkalian(x,y);
			nonstatic.pembagian(x,y);
			nonstatic.sederhana(x,y);
			return 0;
      }
		
