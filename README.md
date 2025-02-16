#include <stdio.h>
#include <stdlib.h>
int main(){
    int *arr,n;
    printf("enter a number of elements: ");
    scanf("%d",&n);
    arr=(int *)calloc(n,sizeof(n));
    if(arr==NULL){
        printf("Memory Allocation failed\n");
        return 1;
    }
    printf("Enter %d elements\n",n);
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    printf("Entered elements are: \n");
    for(int i=0;i<n;i++){
        printf("%d ",arr[i]);
    }
    printf("\n");
    free(arr);
    return 0;
}
