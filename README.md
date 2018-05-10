# brilhante-waffle
#include <stdio.h>
#include <locale.h>

void main() {
	
	setlocale(LC_ALL, "");
	
	char cargo;
	
	float salario;
	
	printf("Informe seu cargo: \n");
	printf("1- Arquiteto \n");
	printf("2- Engenheiro Civil \n");
	printf("3- Eng. Produção \n");
	printf("4- Cientista da Computação \n");
	scanf("%i", &cargo);
	
	
	printf("Informe seu salário: \n");
	scanf("%f", &salario);
	
	switch (cargo){
		
		case  1:
			printf("\n Arquiteto");
			salario = salario + salario * 0.04;
			
				if (salario >=2800){
				 salario = salario - salario * 0.15;
				 printf("\n Salário liquido = %.2f", salario);
			}else{
				 printf("\n Salario %.2f", salario);
			}
			break;
			
		case  2:
			printf("\n Engenheiro Civil");
			break;
		case  3:
			printf("\n Eng. Produção");
			break;
		case  4:
			printf("\n Ciencia da Computação");
			break;
		default:
		    printf("Numero invalido ");	
		    break;
		    
		    
  }


}
