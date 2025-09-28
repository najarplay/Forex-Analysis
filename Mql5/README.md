# Mql5: Scripts para MetaTrader que generan datos

## scrip .01
El primer scrip genere un archivo csv de los datos de mercado OHLC para tener la vela completa del movimiento del mercado (ejem.)

Time	Open	High	Low	Close	Volume
2025.09.19 23:46	1.17426	1.17432	1.17426	1.17427	6
2025.09.19 23:47	1.17427	1.17439	1.17425	1.17439	14

## scrip .02 
Se pulio un poco el codigo quitando la selecion de baras por una selecion de periodo de tiempo , esto ayuda a espesificar los datos

## scrip .03
Se presentaron errores de sobre escritura y la implementacion en las lineas (37, 44, 46) evitan este error 

## scrip .04
Ampliacion de generacion de archivos CSV : Genera todos los archivos del mes desde el dia 01 al ultimo del mes las lineas (18,a,55)
generan la logica para tener la cantidad de dias del mes y el (siclo for) para generar todos los CSV del mes 

## scrip .05 
Reversed : consegimos los datos inversos de un par de divisas para tener los datos completos de divisas 
Orden de nombres :  symbol, year, month, day, initial -> EURUSD-2025-07-01-M 
Ejem: original -> EURUSD-2025-07-01-M
Time	Open	High	Low	Close	Volume
2025.07.01 00:00	1.17849	1.17849	1.17771	1.1780599999999999	6
2025.07.01 00:01	1.1780599999999999	1.1780599999999999	1.17734	1.17798	4
Ejem: reversed -> USDEUR-2025-07-01-M
Time	Open	High	Low	Close	Volume
2025.07.01 00:00	0.848543	0.849105	0.848543	0.848853	6
2025.07.01 00:01	0.848853	0.849372	0.848853	0.848911	4




