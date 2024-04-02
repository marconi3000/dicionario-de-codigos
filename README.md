//Meus primeiros códigos em C

//CÓDIGO PARA ARMAZENAMENTO E IMPRESSÃO DE STRING EM C

int main(void)
{
char name[65];
int dia, mes, ano;

    printf("Entre com seu nome: ");
    gets(name); // Desta maneira consegue armazenar a string com espaços
    printf("Entre com a data do seu aniversario (dd mm aa): "); 
    scanf("%d %d %d", &dia, &mes, &ano);
    printf("%s", name);
    printf(", voce nasceu em %d/%d/%d \o/\n", dia, mes, ano);
    
    getch(); // Usado para coletar e exibir strings com vários caracteres 
    return 0;
}


// CÓDIGO USANDO OPERADORES LÓGICOS COM CONDICIONAIS: 1 PARA VERDADEIRO E 0 PARA FALSO.

#include <stdio.h>
#include <stdlib.h>

// Operadores lógicos com if/else
int main(){
    int n1 = 5, n2 = 10, n3 = 5;
    printf("Numero 1: %d \n", n1);
    printf("Numero 2: %d \n", n2);
    printf("Numero 3: %d \n", n3);
    
    //printf("%d", (n1 == n2) && (n1 == n3));
    
    //printf("\n (n1 == n2) && (n1 == n3) = %d", ((n1 == n2) && (n1 == n3)));
    printf("\nOperador Lógico E(&&) : (n1 == n2) && (n1 == n3) = ");
    
   if (("%d", (n1 == n2) && (n1 == n3)) == 1) {
        printf("Verdadeiro! \n");
    } else {
        printf("Falso!\n");
    }
   
    //printf("\n (n1 == n2) || (n1 == n3) = %d", ((n1 == n2) || (n1 == n3)));
    printf("\nOperador Lógico OU(||) : (n1 == n2) || (n1 == n3) = ");
   
    if (("%d",((n1 == n2) || (n1 == n3))) == 1) {
        printf("Verdadeiro!\n");
    } else {
        printf("Falso!\n");
    }
   
    // printf("\n (n1 < n3) || (n1 > n2) = %d", ((n1 < n3) || (n1 > n2)));
    printf("\nVamos usar esta para negar a proposição abaixo : \n ");
    printf("\nOperador Lógico OU(||) : ((n1 < n3) || (n1 > n2)) = ");
   
    if (("%d", ((n1 < n3) || (n1 > n2))) == 1) {
        printf("Verdadeiro!\n");
    } else {
        printf("Falso!\n");
    }
    
    printf("\nOperador Lógico NÃO(!) : !((n1 < n3) || (n1 > n2)) = ");
   
    if (("%d", !((n1 < n3) || (n1 > n2))) == 1) {
        printf("Verdadeiro!\n");
    } else {
        printf("Falso!\n");
    }
    
}


// CRIANDO UM SWITCH PARA UMA ESCOLHA MOTIVACIONAL

#include <stdio.h>
#include <conio.h>

int main (void )
{
  int valor;
  
  printf ("Digite um valor de 1 a 10: ");
  scanf("%d", &valor);
  
  switch ( valor )
  {
    case 1 :
    printf ("\nÉ melhor você tentar algo, vê-lo não funcionar e aprender com isso, do que não fazer nada. Mark Zuckerberg\n");
    break;
    
    case 2 :
    printf ("\nNossa maior fraqueza é desistir. O caminho mais certo para o sucesso é sempre tentar apenas uma vez mais. Thomas A. Edison\n");
    break;
    
    case 3 :
    printf ("\nO fracasso é uma ótima oportunidade para começar de novo de forma mais inteligente. Henry Ford\n");
    break;
    
    case 4 :
    printf ("\nA melhor forma de prever o futuro é criá-lo.Abraham Lincoln\n");
    break;
    
    case 5 :
    printf ("\nAprenda com o ontem. Viva o hoje. tenha esperança para o amanhã. Albert Einstein\n");
    break;
    
    case 6 :
    printf ("\nSucesso é o acúmulo de pequenos esforços, repetidos dia e noite.Robert Collier\n");
    break;
    
    case 7 :
    printf ("\nVocê não se afoga por cair na água, mas por ficar lá. Ed Cole\n");
    break;
    
    case 8 :
    printf ("\nUma pessoa que nunca cometeu um erro nunca tentou nada novo. Albert Einstein\n");
    break;
    
    case 9 :
    printf ("\nComece de onde você está. Use o que você tiver. Faça o que você puder. Arthur Ashe\n");
    break;
    
    case 10 :
    printf ("\nEducação é a arma mais poderosa que você pode usar para mudar o mundo. BB King\n");
    break;
    
    default :
    printf ("Valor invalido!\n");
  }
  
  getch();
  return 0;
}


// WHILE COMBINADO COM SWITCH NA ESCOLHA DE UMA PROVA

#include <stdio.h>

int main()
{
    int a = 1;
    
    while (a<=10) {
        printf("\nDigite [%d] para realizar a prova [%d]: ", a, a);
        a++;
    }
    
    printf("\nDigite [0] para sair: \n");
    
    scanf("%d", &a);
    
    switch (a) {
        
        case 1:
        printf("Você irá realiza a prova 01! Boa Sorte!");
        break;
        
        case 2:
        printf("Você irá realiza a prova 02! Boa Sorte!");
        break;
        
        case 3:
        printf("Você irá realiza a prova 03! Boa Sorte!");
        break;
        
        case 4:
        printf("Você irá realiza a prova 04! Boa Sorte!");
        break;
        
        case 5:
        printf("Você irá realiza a prova 05! Boa Sorte!");
        break;
        
        case 6:
        printf("Você irá realiza a prova 06! Boa Sorte!");
        break;
        
        case 7:
        printf("Você irá realiza a prova 07! Boa Sorte!");
        break;
        
        case 8:
        printf("Você irá realiza a prova 08! Boa Sorte!");
        break;
        
        case 9:
        printf("Você irá realiza a prova 09! Boa Sorte!");
        break;
        
        case 10:
        printf("Você irá realiza a prova 10! Boa Sorte!");
        break;
        
        case 0:
        printf("Tchau!");
        
        default:
        printf("Digite um número válido!");
    }
    getch();
    return 0;
}

