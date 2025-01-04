# Mathematical-Calculation
A collection of efficient scripts and solutions for mathematical problems, from basic arithmetic to advanced calculations—perfect for learners and developers






/******************************************************************************
                Program for Addition of Two Matrix
*******************************************************************************/
#include <stdio.h>

int main()
{
    int a[5][5],b[5][5],ca,ra,cb,rb,i,j,result[5][5];
    
    printf("Enter No. of row and no. of columnes of matrix a :");
    scanf("%d%d",&ra,&ca);
 
    printf("Enter No. of row and no. of columnes of matrix b :");
    scanf("%d%d",&rb,&cb);
      
   if(ca==cb && ra==rb)
       {         
    printf("Enter Matrix a Elements :");
    for(i=0 ; i<ra ; i++)
       {
         for(j=0 ; j<ca ; j++)
            { 
                scanf("%d",&a[i][j]);
            }
       }   
     printf("Accepted  Matrix a \n\n");
    for(i=0 ; i<ra ; i++)
       {
         for(j=0 ; j<ca ; j++)
            {
                printf("\t%d ",a[i][j]);
            }
            printf("\n");
       }
    printf("\nEnter Matrix b Elements :");
    for(i=0 ; i<rb ; i++)
       {
         for(j=0 ; j<cb ; j++)
            { 
                scanf("%d",&b[i][j]);
            }
       }
       
    
     printf("Accepted  Matrix b \n\n");
    for(i=0 ; i<rb ; i++)
       {
         for(j=0 ; j<cb ; j++)
            {
                printf("\t%d ",b[i][j]);
            }
            printf("\n");
       }
       
     
        for(i=0 ; i<rb ; i++)
              {
               for(j=0 ; j<cb ; j++)
                  { 
                   result[i][j]=a[i][j] + b[i][j];
                 }
              }
       
    
           printf("Addition of a and b Matrix\n\n");
           for(i=0 ; i<rb ; i++)
              { 
               for(j=0 ; j<cb ; j++)
                  {
                   printf("\t%d ",result[i][j]);
                  }
                   printf("\n");
              }
       }
       
       else
       {
           printf("Addition of Matrix is not Possible ...");
       }
     
    return 0;
}




