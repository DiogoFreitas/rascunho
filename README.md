/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

package commerce;

/**
 *
 * @author LABCCET
 */
public class commerce {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
    	char A[]= 'commerce';
    	bool B[8];
	int i,j;
	char aux;
	int count=0;

// inicializa vetor booleano

for(i=0, i<8;i++)
	{  B[i]=0;}

// Percorre vetor
for(j=0;j<8;j++)
{
     aux=A[j];
     for (i=0;i<8;i++)
     {
        if(aux==A[i] && B[i]==0)
	{ count++; B[i]==1;}	
     }
     System.out.println("O caracter " + aux + " = " + count);
     //zere
     count=0;
}

/*Para armazenar: pense em uma pilha que armazene a quantidade de vezes que aparece. Bastaria consutar "topo". 

Mas a lista encadeada também seria divertido. Novo elo a cada true da comparação do caracter em atribuído a 

variável;
*/	
/* - Véi faz uma struct { int quant; char letra;}, :-P
