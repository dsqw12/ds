#include <stdio.h>
int main(){
    int a[3] [3],i,j,z=0,nz=0;
    for(i=0;i<3;i++)
        for (j=0;j<3;j++){
            printf("Enter the no: ");
            scanf("%d",&a[i] [j]);
        }
        printf("Two dimension ");
    for(i=0;i<3;i++)
    {
        printf("\n");
        for (j=0;j<3;j++)
            printf("%d\t",a[i][j]);
        }
    for(i=0;i<3;i++)
        for (j=0;j<3;j++){
            if (a[i][j]==0)
            z++;
            else
            nz++;
        }
    if (nz>z)
        printf("It is not a sparce matrix");
    else{
    int s[nz][3],k=0;
        for(i=0;i<3;i++)
        for (j=0;j<3;j++){
            if (a[i][j]!=0){
                s[k][0]=i;
                s[k][1]=j;
                s[k][2]=a[i][j];
                k++;
            }}
        printf("Afetr sorting \n");
    for(i=0;i<nz;i++){
        printf("\n");
        for (j=0;j<3;j++)
            printf("%d\t",s[i][j]);
        }
    }
return 0;
}