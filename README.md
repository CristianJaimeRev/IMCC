# IMCC

import java.util.*;

public class ejer2 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		Scanner sc = new Scanner(System.in);
		String sino;
		String si="s";
		String no="n";
		String nombre;
		String Apellido;
		double ALT;
		double PES;
		int EDAD;
		System.out.println("Altura:");
		ALT = sc.nextDouble();

		System.out.println("Peso:");
		PES = sc.nextDouble();
		System.out.println("Nombre:");
		nombre = sc.next();
		Apellido = sc.next();

		System.out.println("EDAD:");
		EDAD = sc.nextInt();
		do {
			int N = 50;

			for (int i = 0; i < N; i++) {

				System.out.print("-");
			}
			System.out.print("\n");
			System.out.println(nombre + " " + Apellido + " (" + EDAD + " Años)");


			int M = 50;

			for (int i = 0; i < M; i++) {

				System.out.print("-");
			}
			System.out.print("\n");

			double IMC=(PES/Math.pow((ALT/100),2));
			System.out.printf( "Índice de Masa Corporal (IMC):  %.2f %n" ,IMC);


			if(IMC<16) {
				String textoFormateado = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado + "Delgadez Severa");
			}	


			if(IMC>=16 && IMC<17) {
				String textoFormateado1 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado1 + "Delgadez moderada");

			}
			if(IMC>=17 && IMC<=18.49) {
				String textoFormateado2 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado2 + "Delgadez aceptable");


			}

			if(IMC>=18.50 && IMC<=24.99) {
				String textoFormateado3 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado3 + "Normal");


			}
			if(IMC==25) {
				String textoFormateado4 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado4 + "Sobrepeso");


			}

			if(IMC>25 && IMC<=29.99) {
				String textoFormateado5 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado5 + "Pre-obeso(Riesgo)");


			}

			if(IMC==30) {
				String textoFormateado6 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado6 + "Obeso");


			}

			if(IMC>30 && IMC<=34.99) {
				String textoFormateado7 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado7 + "Obeso Tipo I (Riesgo Moderado)");


			}

			if(IMC>=35 && IMC<=39.99) {
				String textoFormateado8 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado8 + "Obeso Tipo II (Riesgo Severo)");


			}


			if(IMC>=40) {
				String textoFormateado9 = String.format("%-32s", "Clasificación:");        
				System.out.println(textoFormateado9 + "Obeso Tipo III (Riesgo muy Severo)");


			}
			System.out.print("\n");

			System.out.println("Su rango de peso ideal según la formula del IMC");
			System.out.print("\n");
			System.out.printf("%17s","Peso mínimo");
			System.out.printf("%17s","Peso máximo");
			System.out.print("\n");
			double MIN=Math.pow((ALT/100),2)*18.5;
			double MAN=Math.pow((ALT/100),2)*24.99;
			System.out.printf("%17s",(double)Math.round(MIN * 100d) / 100d +"Kg");
			System.out.printf("%17s",(double)Math.round(MAN * 100d) / 100d + "Kg");

			System.out.printf("\n");

			System.out.println("Desea continuar(s/n)");
			sino = sc.next();
		}while(sino==si); {
			if(sino==no && sino != si); 

			

				System.out.println("Altura:");
				ALT = sc.nextDouble();

				System.out.println("Peso:");
				PES = sc.nextDouble();
				System.out.println("Nombre:");
				nombre = sc.next();
				Apellido = sc.next();

				System.out.println("EDAD:");
				EDAD = sc.nextInt();

			
					

			
			
			
			
			}

		System.out.println("Hasta luegorrrr");


	}

}
