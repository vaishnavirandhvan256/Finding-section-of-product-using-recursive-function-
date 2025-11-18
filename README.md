# Finding-section-of-product-using-recursive-function-



// Online C compiler to run C program online
#include <stdio.h>

   int fun(int n){
   if(n==1){
       return 1;
   }
   else {
   
   return(n+fun(n-1));
   }
   }
 int main(){
     int a;
     printf("Enter a product number:");
     scanf("%d", &a);
     
    int result=fun(a);
   
   if(result <=5123){
       printf("product from A section");
   }else
   if(5123<result&&result<=20150){
       printf("product from B section");
   }else
   if(20150<result&&result<=45350){
       printf("product from C section");   
   }else
   if(45350<result&&result<=80360){
       printf("product from D section");   
   }else
   if(80360<result&&result<=125250){
       printf("product from 3rd floor");   
   }
   else{
       printf("Please enter correct product number");
   }
           
   
return 0;

}
