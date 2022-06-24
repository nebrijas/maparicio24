# AD3

Esta es la **actividad dirigida 3**, que consiste en hacer un ejercicio de programación literaria aprovechando el código que hemos usado en programación con **Python** y dónde realizamos *web scrapping*. A continuación pongo el **código fuente**:

## CODIGO

A continuacion el codigo a implementar:

```
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored
resultados = []
req = requests.get("https://resultados.elpais.com")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')
tags = soup.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')
tags = soup2.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req3 = requests.get("https://elpais.com/opinion")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup3 = BeautifulSoup(req3.text, 'html.parser')
tags = soup3.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')
tags = soup4.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')
tags = soup5.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')
tags = soup6.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')
tags = soup7.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')
tags = soup8.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')
tags = soup9.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')
tags = soup10.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')
tags = soup11.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')
tags = soup12.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')
tags = soup13.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req14 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup14 = BeautifulSoup(req14.text, 'html.parser')
tags = soup14.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')
tags = soup15.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req16 = requests.get("https://elpais.com/television/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup16 = BeautifulSoup(req16.text, 'html.parser')
tags = soup16.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')
tags = soup17.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
os.system("clear")
print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))
str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))
print(colored("Igualdad", 'green', attrs=['bold']))
str_match = [s for s in resultados if "igualdad" in s]
print("\n".join(str_match))
print(colored("Mujeres", 'green', attrs=['bold']))
str_match = [s for s in resultados if "mujeres" in s]
print("\n".join(str_match))
print(colored("Mujer", 'green', attrs=['bold']))
str_match = [s for s in resultados if "mujer" in s]
print("\n".join(str_match))
print(colored("Brecha salarial", 'green', attrs=['bold']))
str_match = [s for s in resultados if "brecha salarial" in s]
print("\n".join(str_match))
print(colored("Machismo", 'green', attrs=['bold']))
str_match = [s for s in resultados if "machismo" in s]
print("\n".join(str_match))
print(colored("Violencia", 'green', attrs=['bold']))
str_match = [s for s in resultados if "violencia" in s]
print("\n".join(str_match))
print(colored("Maltrato", 'green', attrs=['bold']))
str_match = [s for s in resultados if "maltrato" in s]
print("\n".join(str_match))
print(colored("Homicidio", 'green', attrs=['bold']))
str_match = [s for s in resultados if "homicidio" in s]
print("\n".join(str_match))
print(colored("Género", 'green', attrs=['bold']))
str_match = [s for s in resultados if "género" in s]
print("\n".join(str_match))
print(colored("Asesinato", 'green', attrs=['bold']))
str_match = [s for s in resultados if "asesinato" in s]
print("\n".join(str_match))
print(colored("Sexo", 'green', attrs=['bold']))
str_match = [s for s in resultados if "sexo" in s]
print("\n".join(str_match))
```

## Programación literaria

### Librerias internas

Estas son librerias que ya vienen instaladas con el python y que pueden ser invocadas sin ninguna instalacion externa.
- `time`
- `csv`
- `re`
- `os`

#### Librerías externas
- `requests`
- `bs4`
- `pandas`
- `termcolor`

### Comando para instalar librerias externas

```python
pip install requests bs4 pandas termcolor
```

### Invocacion o importancion de las librerias en el codigo

```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored
```

### Explicacion del codigo

El codigo consiste en realizar **scrapping** a distintas paginas donde se busca encontrar todos los titulos que tienen la etiqueta h2 de html en la pagina. 
Estos datos se guardan en la variable tipo lista:
```python
resultados = []
```

El codigo que se utiliza para realizar el **scrapping** es el siguiente:
```python
req = requests.get("<URL>")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')
tags = soup.findAll("h2")
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

NOTA: <URL>, es donde ira las URL a realizar el scrapping.
    Las URL a realizar scrapping son las siguiente:
- https://resultados.elpais.com
- https://elpais.com/internacional
- https://elpais.com/opinion
- https://elpais.com/espana/
- https://elpais.com/economia/
- https://elpais.com/educacion/
- https://elpais.com/clima-y-medio-ambiente/
- https://elpais.com/ciencia/
- https://elpais.com/cultura/
- https://elpais.com/babelia/
- https://elpais.com/deportes/
- https://elpais.com/tecnologia/
- https://elpais.com/gente/
- https://elpais.com/television/
- https://elpais.com/eps/
    
Posterior a esto se realizara una categorizacion de los temas usando palabras claves de la siguiente forma:
```python
print(colored("Feminismo", 'green', attrs=['bold']))
str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))
```
Para el caso de este codigo se busca encontrar la palabra feminismo en los titulos.

Se realizo la categorizacion con las siguientes categorias:
    - Feminismo
    - Igualdad
    - Mujeres
    - Mujer
    - Brecha salarial
    - Machismo
    - Violencia
    - Maltrato
    - Homicidio
    - Género
    - Asesinato
    - Sexo