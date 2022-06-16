#crea una matriz filaXcolumna
matriz=[[1,1,1,1],[2,3,4,5],[6,7,8,9],[10,11,12,13]]
print("LA matriz es: ",matriz)

#sacar una fila de la matriz
fila = matriz[1:2]
print("La fila es: ",fila)

# sacar una columna de la matriz
columna=[x[1] for x in matriz]
print("La columna es: ",columna)

#suma de una fila
suma_f=0
for valor in matriz[1:2]:  # de esta manera sale la fila tambien COMPRESION DE LISTAS
    print("El valor es: ",valor)
    for i in valor:
        suma_f=suma_f+i
print("La suma de la fila es: ",suma_f)


#suma de una columna
suma_c=0
for valor in matriz:
    suma_c=suma_c+valor[1]  #suma los valores dela columna 0
print("La suma de la columna es: ",suma_c)

# SACAR EL NUMERO MAYOR DE LA matriz
mas_alta = -100

for A in matriz:  # saca la fila (0) A
    #print(A)
    for B in A:   #saca el primer valor de la fila 0, es decir la columna B en pocas(A,B)
        #print(B)
        if B>mas_alta:  #el valor erifica que sea mas alto 
            mas_alta=B   # reemplaza el nuevo valor mas alto
print("El numero mas alto es: ",mas_alta)

# cuantas veces se repite el 1 en la primera fila
repetido=0
for A in matriz[0:1]:
    for i in A:
        #print(i)
        if i==1:
            repetido=repetido+1
print("Cantidad de unos es",repetido)
