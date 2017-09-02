# Calculadora
/*Ian da Silva e Matheus Bispo*/
/*02/09/2017*/
#include <stdio.h>

int main(int argc, char **argv)
{
    /*Declaração de variáveis*/

    int  o, soma=0, d, aux;
    char p;

    /*Descrição de valores e Operadores*/

    printf("Digite um numero: ");
    scanf("%d",&soma);


    /*Inicio da Repetição e procedimento de formulação do calculo*/

    while(d!=0){

    printf("Digite um operador: ");
    scanf(" %c",&p);
    printf("Digite um numero: ");
    scanf("%d",&d);

    if(p == '+')
    {
        soma = soma + d;
    }else if(p =='-')
    {
        soma = soma - d;
    }else if(p == '*')
    {
        soma = soma * d;
    }else if(p == '/')
    {
        soma = soma / d;
    }else if(p == '^')
    {

    /*Formula da Potência*/

    aux=soma;
    for(o=1;o<d;o++)
    {
        soma = soma * aux;
    }

    }

    /*Resultado das Operações*/

    printf("%d\n",soma);

    /*Retorno para o segmento de valores até o primeiro numero ser zero*/




    }



    return 0;
}
