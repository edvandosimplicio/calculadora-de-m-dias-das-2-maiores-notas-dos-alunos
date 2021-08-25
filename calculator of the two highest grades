#include <stdio.h>
#include <string.h>

typedef struct {
      char nome[20];
      int matricula;
      float n1,n2,n3;

}Escola;


int main(void) {

      Escola escola[20];
      int c=0,resp,i;
      float media;
do {
      setbuf(stdin, 0);
      printf("-----CALCULADORA DE MÉDIA DOS ALUNOS------\n");
      printf("digite seu nome: ");
      fgets(escola[c].nome, 20, stdin);
      escola[c].nome[strcspn(escola[c].nome, "\n")] = '\0';

      setbuf(stdin, 0);
 
      printf("Digite sua matricula:");
      scanf("%d",&escola[c].matricula);

      printf("Digite a 1ª nota do aluno:");
      scanf("%f",&escola[c].n1);

      printf("Digite a 2ª nota do aluno:");
      scanf("%f",&escola[c].n2);

      printf("Digite a 3ª nota do aluno:");
      scanf("%f",&escola[c].n3);

if(escola[c].n1 >= escola[c].n2 && escola[c].n3 >= escola[c].n2){

      media = (escola[c].n1+escola[c].n3)/2;
}

if (escola[c].n2 >= escola[c].n1 && escola[c].n3 >= escola[c].n1){

      media= (escola[c].n2+escola[c].n3)/2;

}
if (escola[c].n1 > escola[c].n3 && escola[c].n2 > escola[c].n3){

      media=(escola[c].n1+escola[c].n2)/2;

}


printf("Deseja cadastrar mais um aluno? 1-sim / 2-não");
scanf("%d",&resp);

c++;
}while(resp==1);
 
 if (resp == 2){ 
 for(i=0; i<c; i++){

  printf("\n└───────────┴──────────────────────┴──────────────────────┴──────┴──────┴─────────┴────────────┘");

  printf("\n\nEmpresa Legal\n");
  printf("\nListagem Geral\n");
  printf("┌───────────┬──────────────────────┬────────┬────────┬────────┬─────────┬─┐");
  printf("\n│ Matricula │ Nome                 │ nota1  │ nota2  | nota3  | media   |");
  printf("\n├───────────┼──────────────────────┼────────┼────────┼────────┼─────────┤");
  for(i=0; i<c; i++) {
  
    printf("\n│ %-9d │ %-20s │ %-6.2f | %-6.1f | %-6.1f | %-7.1f |", escola[i].matricula, escola[i].nome, escola[i].n1, escola[i].n2, escola[i].n3, media);
  }

  printf("\n└───────────┴──────────────────────┴────────┴────────┴────────┴─────────┴─┘");


 }
 }

return 0; 
}
