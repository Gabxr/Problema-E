#include <stdio.h>     
#include <stdlib.h>



int main (){



do {
int n,p,d;

printf("Quantos numeros entrarao na contagem final? ");

scanf("%d",&n);

printf("\nPrimeiro numero: ");

scanf("\n%d",&p);

printf("\nSegundo numero: ");

scanf("\n%d",&d);

int cont=0;



printf("\n------------------------------------\n");





for (int i=1; i<n+1; i++){

int x,y,a,b;



cont=cont+1;

x=i%p;	

y=i%d;

a=(i-p)%10;

b=(i-d)%10;



if ((x==0) || (y==0) || (a==0) || (b==0))

{

printf("Cafufa");

		

		if (i<n)

		printf(", ");

		else

		printf(".");



} else 

{

printf("%i",i);

		if (i<n)

		printf(", ");

		else

		printf(".");

}

}

char resposta;

printf("\n\nDeseja testar outra vez? ");
printf("\n('s' para continuar/qualquer tecla para sair): ");
scanf("\n%c",&resposta);
if (resposta != 's'){
	exit(0);
}
} while (1);




return 0;

}
