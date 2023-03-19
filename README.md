# itsa-no.7
#include <iostream>
  
using namespace std;
 
int main()
{
  
    int n;
    cin >> n;
    while (n--)
    {
        int a1,a2,b1,b2; //設定變數
        char w; 
        cin>>w>>a1>>a2>>b1>>b2;
        switch(w)  //根據所輸入的符號來執行下列的步驟
       {
            case '+':cout<<a1+b1<<" "<<a2+b2<<"\n";break; //若是加號，則將其相加，輸出結果
            case '-':cout<<a1-b1<<" "<<a2-b2<<"\n";break; //若是減號，則將其相減，輸出結果
            case '*':cout<<a1*b1-a2*b2<<" "<<a2*b1+a1*b2<<"\n";break; //若是乘號，則將其相乘，並通過運算後，輸出結果
            case '/':cout<<(a1*b1+a2*b2)/(b1*b1+b2*b2)<<" "<<(a2*b1-a1*b2)/(b1*b1+b2*b2)<<"\n";break; //若是除號，則將其相除，並通過運算後，輸出結果
        }
    }
     
}
