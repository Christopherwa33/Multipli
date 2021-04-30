# Multiplipackage main;

import java.util.Scanner;

public class EsercizioGuidatoFor {

	public static void main(String[] args) {
		/*
		 Scrivere un programma che letti dei numeri da tastiera
		 restituisca solo i multipli di tre
		*/
		Scanner tastiera = new Scanner(System.in);
		
		System.out.println("Quanti numeri vuoi inserire?");
		int dim = Integer.parseInt(tastiera.nextLine());
		int [] vettore = new int[dim];
		String risposta = "";
		
		for(int i = 0; i < vettore.length; i++) {
			System.out.println("Inserisci il " + (i+1) + "° numero");
			vettore[i] = Integer.parseInt(tastiera.nextLine());
			
			if(vettore[i] % 3 == 0)
				risposta += vettore[i] + "\n";
		}
		
		System.out.println("I numeri multipli di 3 sono: " + risposta);
		
		tastiera.close();
		

	}

}
