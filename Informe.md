**Universidad Peruana de Ciencias Aplicadas**
=============================================

# CC42 – Complejidad Algorítmica

# Trabajo Final



# Integrantes

| Integrantes | Codigo | Usuario | Correo | 
|---|---|---|---|
| Jorge Arturo Tafur Pastor | U202015558 | JorgeTafur | u202015558@upc.edu.pe |

# Link del repositorio:

https://github.com/JorgeTafur/TF-202015558

# Profesor:
Luis Martin Canaval Sánchez 

**2022 – 1**
============

# ÍNDICE
### 1. INTRODUCCIÓN
### 2. MAPA VISUAL CON NODOS 
### 3. LISTA DE CALLES UTILIZADAS
### 4. REPOSITORIO Y DESCRIPCIÓN DE LA CODIFICACIÓN
### 5. CONCLUSIONES


# 1. RESUMEN EJECUTIVO 

##### El trabajo final es la continuación de lo realizado en el trabajo parcial, consiste en construir nuestro propia aplicación de caminos óptimos al estilo “waze”, es decir un sistema que nos permita encontrar la ruta más corta entre 2 puntos en una ciudad. La ciudad está representada por un grafo que fue el resultado de su trabajo parcial. El trabajo parcial consistió en elaborar un grafo para representar una ciudad o una porción o distritos de una ciudad grande como Lima, en este caso del distrito de San Borja.

# 2. MAPA VISUAL CON NODOS
##### Se eligió utilizar la herramienta brindada por Google Maps para la elaboración del mapa y tenerlo de referencia para la elaboración del grafo y algoritmos

https://www.google.com/maps/d/u/0/edit?mid=10YmeKCoY1-kNc_U00xwcjFf8B6iAUyvG&ll=-12.09966890248742%2C-77.00309358033083&z=15

# 3. LISTA DE CALLES UTILIZADAS
##### Presento una lista de calles recogidas de la herramienta mencionada, utilizado para las listas de adyacencia del proyecto:

* n	nombre de calle
* 0	Avenida Canadá 1
* 1	Avenida Canadá 2
* 2	Avenida Luis Aldana 1
* 3	Avenida Luis Aldana 2
* 4	Calle Del Lenguaje
* 5	Calle de las Letras
* 6	Avenida del Aire 1
* 7	Avenida del Aire 2
* 8	Calle De La Prosa
* 9	Avenida De La Poesía 1
* 10	Avenida De La Poesía 2
* 11	Avenida Aviación 1
* 12	Avenida Aviación 2
* 13	Calle Cerro Colorido
* 14	Calle del Comercio
* 15	Cerro Blanco
* 16	Calle Cerro Sechín
* 17	Calle Cerro Centinela
* 18	Calle C-5
* 19	Jirón de la Historia
* 20	Calle Naturaleza
* 21	Calle Cultura
* 22	Avenida de la Arqueología 1
* 23	Avenida de la Arqueología 2
* 24	Calle de las Bellas Artes
* 25	Calle De la Ciencia
* 26	Calle de la Técnica 1
* 27	Calle de la Técnica 2
* 28	Calle Artesania
* 29	Avenida San Luis 1
* 30	Avenida San Luis 2
* 31	Jirón Horacio Ballón
* 32	Calle Nicanor Arteaga
* 33	Avenida Julio Bailetti 1
* 34	Avenida Julio Bailetti 2
* 35	Calle Pinela
* 36	Calle Estremadoyro
* 37	Calle Parraga
* 38	Calle Esteban Bentarelli
* 39	Avenida Augusto de la Rosa Toro 1
* 40	Avenida Augusto de la Rosa Toro 2
* 41	Jirón Mayor José Urdanivia
* 42	Jirón Jorge Aprile
* 43	Calle Mario Florian
* 44	Calle General Francisco O’Connor
* 45	Calle Enrique Pastor
* 46	Calle Manuel Scorza
* 47	Calle José Astudillo
* 48	Calle Leónidas Yerovi
* 49	Calle Infante de la Torre
* 50	Calle Capitán Daniel Muñoz
* 51	Calle Abelardo Solis
* 52	Calle José Jimenez Borja
* 53	Jirón Eduardo Lizarzaburu
* 54	Calle Arévalo
* 55	Calle Alberto Hidalgo
* 56	Calle General Fortunato
* 57	Calle Pascual Quiñones
* 58	Calle Octavio Mena
* 59	Calle Alberta Ureta
* 60	Calle Jorge Ezeta
* 61	Jirón Enrique Oliveros
* 62	Jirón Víctor Velezmoro
* 63	Calle Ismael Frias
* 64	Calle Miranda
* 65	Calle General Miguel Cerna
* 66	Avenida Circunvalación 1
* 67	Avenida Circunvalación 2
* 68	Avenida Javier Prado Este 1
* 69	Avenida Javier Prado Este 2
* 70	Vía Expresa Avenida Javier Prado Este 1
* 71	Vía Expresa Avenida Javier Prado Este 2
* 72	Jirón Ucello
* 73	Calle Morelli
* 74	Calle Bernini
* 75	Calle Johanes Vermeer
* 76	Calle Carpaccio
* 77	Calle Regoyos
* 78	Calle Carlo Crivelli
* 79	Calle Holbein
* 80	Calle Sisley
* 81	Avenida de las Artes Norte
* 82	Calle Hals
* 83	Calle Portinari
* 84	Jirón Benlliure
* 85	Jirón Tasso
* 86	Calle Vasari
* 87	Calle Derain
* 88	Calle Berta Morisort
* 89	Jirón Tiziano Vecellio
* 90	Calle Botticelli
* 91	Calle Goya
* 92	Calle Degas
* 93	Calle Bellini
* 94	Calle Luiggi Barsato
* 95	Calle Cezzane
* 96	Calle Zurbaran
* 97	Calle Boccioni
* 98	Calle Conti
* 99	Calle Tintoretto
* 100	Jirón Leonardo da Vinci
* 101	Calle Giotto
* 102	Calle Rafael
* 103	Calle Donatello
* 104	Calle Miguel Angel
* 105	Calle Murillo
* 106	Calle Picasso
* 107	Calle Rembrandt
* 108	Calle Velasquez
* 109	Calle Rubens
* 110	Calle Matisse
* 111	Calle Rivera
* 112	Jirón Bronzino
* 113	Calle Van Gogh
* 114	Calle Anthon Van Dyck
* 115	Calle Bartolome Bermejo
* 116	Calle Alonso del Arco
* 117	Jirón Toulose Lautrec
* 118	Calle Breton
* 119	Calle Monet
* 120	Calle Millet
* 121	Calle José María Sert
* 122	Jirón Salvador Dali
* 123	Calle Francisco de Ribalta
* 124	Calle Joaquín Sorolla
* 125	Calle Dominguez
* 126	Calle Dore
* 127	Calle Redon
* 128	Calle Pradilla
* 129	Calle Delacroix
* 130	Calle Rousseau
* 131	Calle Verrocchio
* 132	Calle Carzou
* 133	Calle Cavallini
* 134	Jirón Los Sauces 1
* 135	Calle Sauces
* 136	Calle Pissarro
* 137	Calle Corot
* 138	Calle Jean Louis Forain
* 139	Calle Chardin
* 140	Calle Gauguin
* 141	Calle Hassinger
* 142	Calle Holbein
* 143	Calle Infante
* 144	Calle Jean Louis Forain
* 145	Calle Van de Velde
* 146	Calle Baron F de Gerard
* 147	Calle Dupre
* 148	Calle Benton
* 149	Calle Severini
* 150	Jirón Stephen Crane
* 151	Jirón Los Sauces 2
* 152	Calle Poussin
* 153	Avenida Boulevard de Surco 1
* 154	Calle 41
* 155	Jirón 2
* 156	Calle 9
* 157	Calle 8
* 158	Calle 7
* 159	Calle 6
* 160	Calle 5
* 161	Calle 4
* 162	Calle 3
* 163	Calle 41
* 164	Jirón Paseo del Bosque
* 165	Calle Rigios
* 166	Calle Treinta
* 167	Calle 31
* 168	Calle 35
* 169	Calle 33
* 170	Calle 36
* 171	Avenida Velasco Astete 1
* 172	Avenida Velasco Astete 2
* 173	Jirón 10
* 174	Calle 24
* 175	Calle 25
* 176	Calle 29
* 177	Calle 1
* 178	Calle 26
* 179	Calle 27
* 180	Calle 17
* 181	Carretera Panamericana Sur 1
* 182	Carretera Panamericana Sur 2
* 183	Avenida San Borja Norte 1
* 184	Avenida San Borja Norte 2
* 185	Avenida Del Parque Norte
* 186	Calle Paul Dubois
* 187	Jirón Pietro Torrigiano
* 188	Jirón Frederick Remington
* 189	Jirón López de Ayala
* 190	Calle Berruguette
* 191	Calle Canova
* 192	Calle Españoleto
* 193	Calle Eduardo Rosales
* 194	Calle Guardi
* 195	Calle Fragonard
* 196	Calle Crepi
* 197	Calle Papini
* 198	Avenida de las Artes Sur
* 199	Calle Gaddi
* 200	Calle Duccio
* 201	Calle Pisano
* 202	Calle Reni
* 203	Calle Renoir
* 204	Calle Matier
* 205	Calle Luigi Pirandello
* 206	Calle Perugino
* 207	Jirón Pietro Marchand
* 208	Calle Reynolds
* 209	Calle Simoni
* 210	Calle Monti
* 211	Calle Donizetti
* 212	Calle Manuel de Falla
* 213	Calle Ravel
* 214	Calle Johann Strauss
* 215	Calle Orozco
* 216	Calle Fray Angelico
* 217	Calle Tiepolo
* 218	Calle Veronesse
* 219	Calle Correggio
* 220	Calle Carla Schumann
* 221	Calle Enrique Granados
* 222	Calle Beethoven 1
* 223	Calle Nicolo Paganini
* 224	Jirón Joaquin Valverde
* 225	Calle Verdi
* 226	Calle Wagner
* 227	Jirón El Greco
* 228	Calle Andrea Del Sarto
* 229	Calle Maurice Utrillo
* 230	Calle Dante Gabriel Rosetti
* 231	Calle Claude Monteverdi
* 232	Calle Claude Debussi
* 233	Calle Mauricio Casatti
* 234	Calle Johannes Brahms
* 235	Calle Beethoven 2
* 236	Calle Liszt
* 237	Jirón Juan Gris
* 238	Calle Preising
* 239	Calle Amadeo Mozart
* 240	Calle Bottger
* 241	Calle Schipper
* 242	Calle Mayer
* 243	Avenida El Derby
* 244	Calle 20 1
* 245	Calle 20 2
* 246	Avenida Buena Vista 1
* 247	Avenida Buena Vista 2
* 248	Avenida San Borja Sur 1
* 249	Avenida San Borja Sur 2
* 250	Avenida José Galvez Barrenechea 1
* 251	Avenida José Galvez Barrenechea 2
* 252	Avenida del Parque Sur 1
* 253	Avenida del Parque Sur 2
* 254	Calle Ossip Zadkin
* 255	Calle Copernico
* 256	Jirón Gozzoli Sur
* 257	Calle Dalton
* 258	Calle Leohard Euler
* 259	Jirón Philipp Von Leonard
* 260	Calle John Neper
* 261	Calle Gaspar Monge
* 262	Jirón Alexander Fleming
* 263	Jirón Alberto Barajas
* 264	Calle Amadeo Avogadro
* 265	Jirón Andreas Vesalio
* 266	Jirón Eduardo Ordoñez
* 267	Jirón Mercator
* 268	Jirón Ernesto Rutherford
* 269	Calle Oersted
* 270	Calle Claudio Galeno
* 271	Jirón Joseph Thompson
* 272	Avenida A
* 273	Calle Gregorio Marañon
* 274	Calle Francesco Redi
* 275	Jirón Isaac Albeniz
* 276	Jirón Gregorio Marañón
* 277	Jirón Hermano Lobo
* 278	Jirón Isaac Albeniz
* 279	Calle Sibelius
* 280	Calle las Magnolias
* 281	Jirón Arquitecto Fernando Echeandia
* 282	Calle Tapia Garcia
* 283	Calle Paul Linder 1
* 284	Calle Paul Linder 2
* 285	Calle Grana
* 286	Jirón Enrique Seoane
* 287	Calle Manuel Piqueras
* 288	Calle Benitez
* 289	Calle Profesor Jorge Muelle
* 290	Calle Montero
* 291	Calle Alvarez Calderon
* 292	Calle Vargas Prada
* 293	Calle Eduardo Orrego Villacorta
* 294	Calle Urquiaga
* 295	Avenida Malachowsky 1
* 296	Avenida Malachowsky 2
* 297	Calle Claude Sahut
* 298	Calle Emilio Harth Terre 1
* 299	Calle Emilio Harth Terre 2
* 300	Avenida Miguel Iglesias 1
* 301	Avenida Miguel Iglesias 2
* 302	Calle 31
* 303	Calle Ramsey
* 304	Calle Nicolas de Pierola
* 305	Calle San Juan de Miraflores
* 306	Calle General Belisario Suarez
* 307	Calle Justo Pastor Davila
* 308	Jirón Daniel Alcides Carrion
* 309	Calle Santa Rosa
* 310	Jirón Gozzoli Norte
* 311	Calle Puccini
* 312	Calle Faure
* 313	Calle Fedorovich Stravinski
* 314	Avenida Joaquín de la Madrid 1
* 315	Avenida Joaquín de la Madrid 2
* 316	Calle Saint Saenz
* 317	Calle Pablo Casals
* 318	Calle Maestro Arrieta
* 319	Calle Alfa
* 320	Calle Gamma
* 321	Calle Omega
* 322	Calle Geminis
* 323	Calle Delta
* 324	Calle Beta
* 325	Calle Sigma
* 326	Calle Epsilon
* 327	Jirón Moisés Mendelssohn
* 328	Calle Otto Muller
* 329	Calle Joaquin Turina
* 330	Calle Argenta
* 331	Jirón Maestro Barbieri
* 332	Calle Jacinto Guerrero
* 333	Calle Andres Segovia
* 334	Calle Chueca
* 335	Calle Pablo Usandizaga
* 336	Jirón Romero Hidalgo
* 337	Jirón Pietro Mascagni
* 338	Calle Amadeo
* 339	Calle Joachim Moser Hans
* 340	Calle Toselli
* 341	Jirón Alejandro Scarlatti
* 342	Calle Tchaicovski
* 343	Calle Franz Schubert
* 344	Jirón Batrich Bozovich
* 345	Calle Leo Baumann
* 346	Calle John Hassinger
* 347	Calle Schrader
* 348	Avenida Boulevard de Surco 2
* 349	Avenida de la Floresta
* 350	Avenida del Pinar 1
* 351	Calle Varese
* 352	Calle Pisa
* 353	Calle Sicilia
* 354	Avenida del Pinar 2
* 355	Calle Melissa
* 356	Calle Palermo
* 357	Calle Trinidad
* 358	Calle Venecia
* 359	Jirón la Pradera
* 360	Calle Florencia
* 361	Calle Esmeralda 1
* 362	Calle Esmeralda 2
* 363	Calle Esmeralda 3
* 364	Calle Buen Retiro
* 365	Calle Andalucía
* 366	Calle Matamoros
* 367	Avenida Alejandro Velasco Astete 1
* 368	Avenida Alejandro Velasco Astete 2
* 369	Calle Bielovucic Cavalier 1
* 370	Calle Bielovucic Cavalier 2
* 371	Calle Pacaritambo
* 372	Calle Galeon
* 373	Jirón Hermano Lobo
* 374	Alameda Picaflores 1
* 375	Alameda Picaflores 2
* 376	Calle Dorado
* 377	Calle Bello Horizonte
* 378	Calle Los Recuerdos
* 379	Calle Las Garzas
* 380	Calle Mayorazgo
* 381	Calle las Canarias
* 382	Calle Vicente Morales Duarez
* 383	Avenida Angamos 1
* 384	Avenida Angamos 2
* 385	Auxiliar Avenida Angamos 1
* 386	Auxiliar Avenida Angamos 2
* 387	Calle Pascal
* 388	Calle Andrea del Sarto
* 389	Avenida Primavera 1
* 390	Avenida Primavera 2
* 391	Auxiliar Avenida Primavera 1
* 392	Auxiliar Avenida Primavera 2
* 393	Avenida Guardia Civil 1
* 394	Avenida Guardia Civil 2
* 395	Museo de la Nación
* 396	Calle Ezaine
* 397	Calle Rousseau Norte
* 398	Auxiliar Avenida Circunvalación
* 399	Calle Hadraza
* 400	Calle Durero
* 401	Calle Hualgayoc
* 402	Calle 39
* 403	Calle 23
* 404	Calle 22
* 405	Calle Luini
* 406	Avenida San Borja Norte 3
* 407	Jirón Fray Luis de León

# 4. REPOSITORIO Y DESCRIPCIÓN DE LA CODIFICACIÓN

##### Para el trabajo final se utilizó el uso de un repositorio público en GitHub.
##### Link del repositorio: https://github.com/JorgeTafur/TF-202015558

##### Se utilizaron los algoritmos Dijkstra y BFS para el camino más óptimo y el alternativo respectivamente
##### Se utilizó lectura de datos de archivo y población en listas como lista de adyacencia y con tuplas para el procesamiento de algoritmos
##### Se operó datos numéricos como el distancia de punto a punto, hora y tráfico de la calle para poder representar bien la autenticidad del objetivo del proyecto

# 5. CONCLUSIONES

##### 1. Fueron indispensables los conocimientos adquiridos dentro del curso para el desarrollo del trabajo final, ya que todos se aplicaron satisfactoriamente.
##### 2. Creemos que todas las competencias del curso de Complejidad Algorítmica fueron completadas a gran medida debido a que se puedo llevar a cabo todas las instancias del trabajo final.
##### 3. Este ha sido un gran entrenamiento para un caso de la vida real, ya que en un futuro podríamos implementar un software similar.
##### 4. Gracias a la realización del trabajo, se aprendieron nuevas cosas que no estaban dentro del curso como el manejo de Hitos e Issues en GitHub y el buen uso del Markdown en un informe.
