// Print the following pattern
// Output:
//   1
//  1 2 3
// 1 2 3 4 5
//1 2 3 4 5 6 7
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the value of n : ";
    cin>>n;
    for(int i=1;i<=n;i++){
        for(int j=1;j<n-i;j++){
            cout<<" ";
        }
        for(int j=1;j<=2*i-1;j++){
            cout<<j;
        }cout<<endl;
    }
}

// Print the following pattern
// Input: n = 4
// Output:
// A
// A B C
// A B C D E
// A B C D E F G
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the value of n : ";
    cin>>n;
    for(int i=1;i<=n;i++){
        for(int j=1;j<n-i;j++){
            cout<<" ";
        }
        for(int j=1;j<=2*i-1;j++){
            cout<<char(j+64);
        }cout<<endl;
    }
}

// Print the following pattern
// Input: n = 4
// Output:
//      A
//    B A B
//   C B A B C
// D C B A B C D
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the value of n : ";
    cin>>n;
    for(int i=1;i<=n;i++){
        for(int j=1;j<=n-i;j++){
            cout<<" ";
        }
        for(int j=i;j>=1;j--){
            cout<<char(j+64);
        }
        for(int q=1;q<=i-1;q++){
            cout<<char(q+1+64);
        }cout<<endl;
    }
}

// Print the following pattern
// Input: n = 4
// Output:
// A B C D E F G
// A B C   E F G
// A B       F G
// A           G
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the Value of n : ";
    cin>>n;
    int m = n-1;
    int nsp=1;
    for(int i=1;i<=2*n-1;i++){
        cout<<char(i+64);
    }
    cout<<endl;
    for(int i=1;i<=m;i++){
        // Stars 
        int a=1;
        for(int j=1;j<=m-i+1;j++){
            cout<<char(a+64);
            a++;
        }
        // Spaces 
        for(int l=1;l<=nsp;l++){
            cout<<" ";
            a++;
        }
        nsp +=2;
        // Stars 
        for(int j=1;j<=m-i+1;j++){
            cout<<char(a+64);
            a++;
        }
        cout<<endl;
    }
}

// Print the following pattern
// Input: n = 4
// Output:
// 1 2 3 4 3 2 1
// 1 2 3   3 2 1
// 1 2       2 1
// 1           1
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the Value of n : ";
    cin>>n;
    int m = n-1;
    int nsp=1;
    for(int i=1;i<=n;i++){
        cout<<i;
    }
    for(int j=n-1;j>=1;j--){
        cout<<j;
    }
    cout<<endl;
    for(int i=1;i<=m;i++){
        // Stars 
        for(int j=1;j<=m-i+1;j++){
            cout<<j;
        }
        // Spaces 
        for(int l=1;l<=nsp;l++){
            cout<<" ";
        }
        nsp +=2;
        // Stars 
        for(int j=m-i+1;j>=1;j--){
            cout<<j;
        }
        cout<<endl;
    }
}

// Print the following pattern
// Input : n = 5
// Output:
// *       *
//  *     * 
//   *   *  
//    * *   
//     *   
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"Enter the value of n : ";
    cin>>n;
    for(int i=1;i<=n;i++){
        for(int j=1;j<=n;j++){
            if(i==j) cout<<"*";
            else cout<<" ";
        }
        for(int j=1;j<=n-1;j++){
            if(i+j==n) cout<<"*";
            else cout<<" ";
        }
        cout<<endl;
    }
}
