Algoritmo formato_matrices
	
	Definir filas, columnas, matriz, i, j Como Entero;
	Definir separador Como Caracter;
	
	separador = "";
	
	Escribir "Digite el numero de filas: "; sin saltar
	Leer filas;
	Escribir "Digite el numero de columnas: "; sin saltar
	Leer columnas;
	
	Dimension matriz[filas,columnas]; // Dimensionamos la matriz
	
	Para i<-0 Hasta columnas Con Paso 1 Hacer // Creamos el separador de filas de acuerdo a la cantidad de columnas
		separador = separador + "---------";
	FinPara
	separador = Subcadena(separador,0,Longitud(separador)-3); // eliminamos los ultimos 3 caracteres para mejor visualizacion de matrices pequenas ( < 10 columnas)
	
	Para i<-0 Hasta filas-1 Con Paso 1 Hacer
		Para j<-0 Hasta columnas-1 Con Paso 1 Hacer
			matriz(i, j) = Aleatorio(0, 1); // Llenamos la matriz con binarios 1/0
		FinPara
	FinPara
	
	Escribir separador;
	Para i<-0 Hasta filas-1 Con Paso 1 Hacer
		Si i <> 0 Entonces
			Escribir separador; // Separamos las filas de la matriz con los guiones
		SiNo
			Para j<-0 Hasta columnas-1 Con Paso 1 Hacer
				Si j <> 0 Entonces
					Escribir "   C", j+1, "   |" Sin Saltar;
				SiNo
					Escribir "      |   C", j+1, "   |" Sin Saltar;
				FinSi;
			FinPara
			Escribir "";
			Escribir separador; // Separador para la primera fila (excepcion)
		FinSi
		Escribir "| F", i+1 Sin Saltar;
		Para j<-0 Hasta columnas-1 Con Paso 1 Hacer
			Escribir  "  |    ", matriz(i, j), " " Sin Saltar;
		FinPara
		Escribir "  |";
	FinPara
	Escribir separador;
FinAlgoritmo
