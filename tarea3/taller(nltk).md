
 Camilo Andres Gativa R. / 161003615


# taller (nltk)

 $ pip install nltk 
esta linea se usa para instalar el paquete nltk.

```python
import nltk
```
en esta linea se importa la libreria

```python
sentence = """At eight o'clock on Thursday morning Arthur didn't feel very good."""
```

En esta linea  "sentence" es una variable de tipo cadena.
la triple comilla nos permite introducir un string.
para ejecutar las funciones del modulo es obligatorio descargar los siguientes paquetes
averaged_perceptron_tagger, maxent_ne_chunker, punkt, treebank, words:
averaged_perceptron_tagger = etiquetadormaxent_ne_chunker = Función de fragmento que hace el trabajo de fragmentación para nosotros.punkt = Éste módulo contiene modelos para la tokenización de textostreebank = Módulo que se vale para etiquetar textos usando expresiones regulareswords = Módulo que procesa una sucesión de palabras y clasifica una parte de la voz

```python
nltk.download()
```


```python
tokens = nltk.word_tokenize(sentence)
```
esta linea separa cada palabra de la oracion que esta guardada como string en sentence

```python
tokens
```
esta linea separa las palabras

```python
tagged = nltk.pos_tag(tokens)
```
esta linea etiqueta palabras segun su gramatica

```python
tagged
```
esta linea muestra cada palabra con su etiqueta

```python
entities = nltk.chunk.ne_chunk(tagged)
```
esta linea identifica las entidades

```python
# entities
```


```python
entities.draw()
```
por ultimo se visualiza las etiquetas de forma grafica