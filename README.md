# -Mallocc-in-C
#include <stdio.h>
#include<stdlib.h>
int main() {
    int *ptr;
    int n;
    scanf("%d",&n);
    ptr=(int*)malloc(n*sizeof(int));
    if(ptr==NULL){
        printf("The array is empty");
    }
    for (int i=0;i<n;i++){
        ptr[i]=i+1;
    }
    for(int i=0;i<n;i++){
        printf("%d",ptr[i]);
    }
    

    return 0;
}
