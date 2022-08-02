# PREENCHIMENTO-DE-MATRIZ-TABULEIRO-XADREZ-COD-JAVA

Deve-se escrever um programa que marque um tabuleiro de xadrez em uma matriz de char, marcando células claras e escuras, como mostrado abaixo:

C

E

C

E

C

E

C

E

E

C

E

C

E

C

E

C

C

E

C

E

C

E

C

E

E

C

E

C

E

C

E

C

C

E

C

E

C

E

C

E

E

C

E

C

E

C

E

C

C

E

C

E

C

E

C

E

E

C

E

C

E

C

E

C

O programa Java abaixo preenche e mostra a matriz corretamente?

public class TabuleiroXadrez {
	public static void main(String[] args) {
		char[][] tabuleiro = new char[8][8];
		
		for(int lin = 0; lin < tabuleiro.length; lin++) {
			for(int col = 0; col < tabuleiro[lin].length; col++) {
				if(col % 2 == lin % 2)
					tabuleiro[lin][col] = 'C';
				else
					tabuleiro[lin][col] = 'E';
			}
		}
		
		for(int lin = 0; lin < tabuleiro.length; lin++) {
			for(int col = 0; col < tabuleiro[lin].length; col++) {
				System.out.printf("%c ", tabuleiro[lin][col]);
			}
			System.out.println();
		}
	}
}

Escolha uma opção:
Verdadeiro 
