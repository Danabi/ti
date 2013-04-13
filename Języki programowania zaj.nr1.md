#JĘZYKI PROGRAMOWANIA

~~~
##Pierwsze zjęcia:

```c
int main() {
  printf (witaj swiecie\n");
}

#include <stdio.h>

int main(){
 double a=3.0,b=7.0;
 printf("Iloczyn %lf x %lf = %.0lf\n",a,b,a*b);
 printf("suma %lf + %lf = %.0lf\n",a,b,a+b);
 printf("roznica %lf - %lf = %.0lf\n",a,b,a-b);
 printf("Iloraz %lf / %lf = %lf\n",a,b,a/b);
 getchar();
 return 0;
}   
```
```c
#include <stdio.h>
#include <math.h>
int main(){
 double r;
 const double pi=M_PI;
 printf("Podaj promien kola\n");
 scanf("%lf",&r);/*  czyta wartosc promienia z kalwiatury */
 printf("Pole wynosi S=%lf, a dlugosc L=%lf",pi*r*r,2*pi*r); 
 
 getchar();
 getchar();
 return 0;
}   
```
```c


#include <stdio.h>

int main(){
 int fahr,celsius; /* deklaracja temperatur */
 int lower, upper, step; /* zakres temperatur i krok */
 lower=0;
 upper=300;
 step=20;
 fahr=lower; /* instrukcja podstawienia */
 while(fahr <= upper){
            celsius=5*(fahr-32)/9;
            printf("%d \t %d\n",fahr,celsius);
            fahr=fahr+step;}
            getchar();
            return 0;
            }
```
```c

#include <stdio.h>

int main(){
double fahr,celsius; /* deklaracja temperatur */
 int lower, upper, step; /* zakres temperatur i krok */
 lower=0;
 upper=300;
 step=20;
 fahr=lower; /* instrukcja podstawienia */
 while(fahr <= upper){
            celsius=5*(fahr-32)/9;
            printf("%5.1lf \t %7.2lf\n",fahr,celsius);
            fahr=fahr+step;}
            getchar();
            return 0;
            }
```
```c

#include <stdio.h>
#define LOWER 0
#define UPPER 300
#define STEP 20
int main(){
int fahr;
for(fahr=LOWER;fahr <= UPPER;fahr=fahr+STEP)
printf("%d3d %6.1lf\n",fahr,(5.0/9.0)*(fahr-32.0));
getchar();
return 0;
}
```
```c

#include <stdio.h>
int main(){
int n1,n2,n3; /*kolejne wyrazy ciagu */
int n; /* numer wyrazu*/
int i; /* licznik */
    do{printf("Podaj numer wyrazu (co najmniej 3):");
         scanf("%d",&n);
         }
         while(n<3);
         n1=n2=1;  /* dwa pierwsze wyrazy ciągu*/
         i=2;
         while(i++<n) /*uwaga, musi być n>2*/
         {
                      n3=n1+n2;
                      n1=n2;
                      n2=n3;
                      }     
     printf("Wyraz o numerze %d ma wartosc %d:",n,n3);       
getchar();
getchar();
return 0;
}
```
```c


#include <stdio.h>


int main(){
int n1,n2,n3; /*kolejne wyrazy ciagu */
int n; /* numer wyrazu*/
int i; /* licznik */
    do{printf("Podaj numer wyrazu (co najmniej 3):");
         scanf("%d",&n);
         }
         while(n<3);
         n1=n2=1;  /* dwa pierwsze wyrazy ciągu*/
         i=2;
         while(i++<n) /*uwaga, musi być n>2*/
         {
                      n3=n1+n2;
                      n1=n2;
                      n2=n3;
                      }     
     printf("Wyraz o numerze %d ma wartosc %d:",n,n3);       
getchar();
getchar();
return 0;
}
```

```c

#include <stdio.h>


#define znak '*' /*znak wypełniania*/
int main(){
int lbwier; /*całkowita liczba wierszy*/
int lw;/* licznik wierszy*/
int lodst; /*liczba odstępów poprzedzających gwiazdkę*/
int j;
printf("ile wierszy?");
scanf("%d",&lbwier);
for(lw=0;lw<lbwier;lw++)
{ lodst=lbwier-lw-1;
for(j=0;j<lodst;j++)putchar(' ');
for(j=0;j<2*lw+1;j++)putchar(znak);
putchar('\n');
}
getchar(); getchar();
}
```

```c

Zadanie 3
#include <stdio.h>
int main(){
    double liczba;
    int n=0;
    double suma=0;
    int licznik=0;
    puts("Podaj ile liczb wczytasz:\n");
    scanf("%d",&n);
    while(licznik<n)
    {    scanf("%lf",&liczba);
         licznik++;
         suma+=liczba;
         }
         printf("Suma = %lf \t , a srednia= %lf",suma,suma/n);
         getchar();getchar();}
```

