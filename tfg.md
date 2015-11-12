
![](http://i.imgur.com/eCb65SE.jpg)

# TRABAJO FIN DE GRADO

## Análisis Regional Del IPRF : Desigualdad Y Progresividad Regional Para España


### Autor

Maximiliano Greco


### Director

Fernando Rodrigo Sauco


--- 

Facultad de Ciencias Económicas y Empresariales
Año 2015

## NOTEBOOK CÁLCULOS

[ENLACE](http://nbviewer.ipython.org/github/mmngreco/Fiscal/blob/master/tfg.ipynb)

## PREGUNTAS

1. Contexto del IRPF 2011
1. El perfil del IRPF en España y CCAA
    + Distribucion de población, España y CCAA
    + Distribucion de los ingresos CCAA
    + Distribucion de declarantes por renta
    + Distribucion de declarantes por CCAA y tg
    + Diferencia entre Ingresos CCAA y Estatal
    + Disperción de Cuota Liquida autonómica y Rentas altas
1. ¿Es el IRPF un impuesto progresivo?
    + Progresividad Local
        * LP
        * ARP
    + Progresividad Global
        * Gini
        * RS
        * Atkinson
1. Caso de Aragón. (sería interesante agregar cataluña o madrid y comparar)
    + Perfil
    + Como se sitúa en presión fiscal
    + Indices
        * LP
        * Gini
        * RS
1. Simulación
    + Hipótesis de partida evolución hasta 2016
        * Evolución BI (PIB o Renta Disponible, media BI)

1. Conclusiones
1. Extensiones del Trabajo
    + Competencia Fiscal

---
# MOTIVACIÓN

La economía pública como disiplina tiene especial interés cuando se trata de corregir los fallos de mercado y promover el correcto funcionamiento de un país. Hoy en día el estado tiene la mayor parte de responsabilidad a la hora de fomentar el crecimietno de un país, gracias a la tendencia creciente en nuestro país en lo relativo a la difusión datos, parece el mejor final de una etapa, la correcta aplicación de los conocimientos adquiridos durante los años de formación en economía a fin de tocar la mayoría de áreas estudiadas.

# METODOLOGÍA

Datos panel IRPF IEF 2011
Varianza estimada boostrap

Software:

Python
- Librerías
- SciPy
- NumPy
- seaborn
- Pandas
- Statsmodels

R
- reldist
- ineq

Desigualdad
Curva de Lorentz
Curva generalizada de Lorentz

# DESCRIPCIÓN PARA ESPAÑA Y CCAA
## DISTRIBUCIÓN DE DECLARANTES POR CCAA

## CODIGOS \[CAMBIAR, INTRODUCIR EN LOS PROPIOS GRÁFICOS]
### Comunidad Autónoma  

1 = Andalucía
2 = Aragón
3 = Principado de Asturias
4 = Illes Baleares
5 = Canarias
6 = Cantabria
7 = Castilla-La Mancha
8 = Castilla y León
9 = Cataluña
10 = Extremadura
11 = Galicia
12 = Comunidad de Madrid
13 = Región de Murcia
16 = La Rioja
17 = Comunidad Valenciana
18 = Ceuta
19 = Melilla

### Tramo de renta

1 = Negativas y cero
2 = De 0,01 a 3.000,00
3 = De 3.000,01 a 6.000,00
4 = De 6.000,01 a 12.000,00
5 = De 12.000,01 a 18.000,00
6 = De 18.000,01 a 30.000,00
7 = De 30.000,01 a 60.000,00
8 = De 60.000,01 a 120.000,00
9 = De 120.000,01 a 240.000,00
10 = De 240.000,01 en adelante

El siguiente gráfico nos muestra la densidad de población sobre el total nacional, por tramos y comunidades autónomas. La población de declarantes en el IRPF, concentra la mayor parte de la población en las comunidades de Cataluña, Andalucía, y Madrid. Aragón se encuentra el noveno entre las comunidades que más declarantes concentran. 

![](imgs/dist_2015-11-09_122758.png)

Por tramos, a simple vista vemos que se ajusta a una distribución normal, es decir, cocentra la mayor densidad en el centro, en este caso se corresponden con los tramos 6 y 7, que pertenecen a los intervalos de 18-30 mil y 30-60 mil respectivamente.

## CURVA DE LORENTZ

Para conocer el grado de concentración de una variable es característico hacerlo median la curva de Lorentz, en las absisas se dibuja el porcentaje de población y en el eje de ordenadas el porcentaje de la variable monetaria de interés. El área entre la bisectriz y la curva de Lorentz es de especial interés ya que nos indica el indice de gini.[1]


![](imgs/lorentz_ingresostrabajo_2015-11-09_122758.png)

![](imgs/lorentz_c731_2015-11-09_122758.png)

![](imgs/lorentz_c730_2015-11-09_122758.png)

### CURVA DE LORENTZ

![](https://media.giphy.com/media/DXzihcl9gQERa/giphy.gif)


![](imgs/lorentz_principales_2015-11-09_122758.png)

## INDICE DE GINI

|VARIABLES|COEFICIENTE|
|:-------------:|:----------:|
|ingresostrabajo|0.461160|
|c690|0.551929|
|c689|0.552380|
|c699|0.697796|
|c698|0.698056|
|c730|0.720683|
|c731|0.725347|
|c620|0.991811|

![](imgs/gini_2015-11-09_122758.png)







---
# IDEAS:

1. ¿Es el gasto público progresivo?
1. Modelo de distribución de la renta, partiendo del ideal y ver su evolución.
1. ¿Son los individuos racionales?
    - Tributación conjunta vs tributación individual para mismas rentas
1. Contraste de Hipótesis:
     - PARA TODOS LOS SUPUESTOS
     - INTERVALO DE CONFIANZA


# NOTAS

## POSIBLES EXTENSIONES DEL TRABAJO
1. ¿Es el gasto público progresivo?
1. Modelo de distribución de la renta, partiendo del ideal y ver su evolución.
1. ¿Son los individuos racionales?
    - Tributación conjunta vs tributación individual para mismas rentas
1. Contraste de Hipótesis:
     - PARA TODOS LOS SUPUESTOS
     - INTERVALO DE CONFIANZA
1. TERNARY PLOT


# BIBLIOGRAFÍA

- Caro, C. D., Fernández, J. O., & Mayo, J. P. (2013). Progresividad y redistribución por fuentes de renta en el IRPF dual. Hacienda pública española, (206), 57-87. http://dialnet.unirioja.es/servlet/articulo?codigo=4604712
- Álvarez, J. A. (2007). Guía del impuesto sobre la renta de las personas físicas. CISS.
- Dept, I. M. F. F. A. (2013). Fiscal Monitor, October 2013. International Monetary Fund.
- Eichhorn, W. (2012a). Models and Measurement of Welfare and Inequality. (W. Eichhorn, Ed.). Berlin, Heidelberg: Springer Science & Business Media. http://doi.org/10.1007/978-3-642-79037-9
- Eichhorn, W. (2012b). Models and Measurement of Welfare and Inequality. (W. Eichhorn, Ed.). Berlin, Heidelberg: Springer Science & Business Media. http://doi.org/10.1007/978-3-642-79037-9
- Galapero Flores, R. (2015). Las rentas del trabajo en el Impuesto sobre la Renta de las Personas Físicas. Estudio jurídico tributario. Dykinson.
- Garcia, S. A. (2010). Diccionario de Economia Publica. ECOBOOK.
- Jorratt, M. (2011). Evaluando la equidad vertical y horizontal en el impuesto al valor agregado y el impuesto a la renta: el impacto de reformas tributarias potenciales. Los casos del Ecuador, Guatemala y el Paraguay.
- López-Laborda, J. (2009). Tributación de rentas a tipo fijo y progresividad de la imposición sobre la renta. F. Picos y S. Díaz de Sarralde (cords.).
- Nolan, B., Salverda, W., Checchi, D., Marx, I., McKnight, A., & Tóth, I. G. (2014). Changing Inequalities and Societal Impacts in Rich Countries. Oxford University Press.
- OECD. (2015). In It Together: Why Less Inequality Benefits All. OECD Publishing. http://doi.org/10.1787/9789264235120-en
- Pfingsten, A. (2012). The Measurement of Tax Progression (Vol. 20). Berlin, Heidelberg: Springer Science & Business Media. http://doi.org/10.1007/978-3-642-82652-8
- Salverda, W., Nolan, B., & Smeeding, T. M. (2009). The Oxford Handbook of Economic Inequality. OUP Oxford.
- Shi, L., Li, S., Sato, H., & Sicular, T. (2013). Rising Inequality in China. (S. Li, H. Sato, & T. Sicular, Eds.). Cambridge: Cambridge University Press. http://doi.org/10.1017/CBO9781139035057
- Silber, J. (2012a). Handbook of Income Inequality Measurement. (J. Silber, Ed.). Dordrecht: Springer Science & Business Media. http://doi.org/10.1007/978-94-011-4413-1
- Silber, J. (2012b). Handbook of Income Inequality Measurement. (J. Silber, Ed.). Dordrecht: Springer Science & Business Media. http://doi.org/10.1007/978-94-011-4413-1
- Stiglitz, J. E. (2003). La economía del sector público. Antoni Bosch editor.

