# CPP
//Majority element!
#include <iostream>

using namespace std;

int main()
{
    int n,majInd=-1;
    int arr[n];
    cout<<"Enter the length of the array : ";
    cin>>n;
    cout<<"Enter the array elements : ";
    for(int i=0;i<n;i++){
        cin>>arr[i];
    }
    
    int c=(n/2);
    for(int i=0;i<=n;i++){
        int count=1;
        for(int j=i+1;j<n;j++){
            if (arr[i]==arr[j]){
                count++;
            }
            
        }
             if(count>c){
             majInd=i;
             }
        
     
    }
    
    if(majInd==-1)
    cout<<"There is no majority element";
    else
    cout<<"Majority element is "<<arr[majInd];

    return 0;
}
