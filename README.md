# Mi primer proyecto

## Pequeño tutorial e introduccion

El formato .md es **MarkDown**

Tenemos 3 tipos de titulos:
- #Titulo Grande
- ##Titulo Mediano
- ###Titulo Chico


Con:
- ** TEXTO**, pones texto en **negrita** 
- * TEXTO*, pones el texto en *cursiva*

**EL TEXTO TIENE QUE TOCAR LOS ASTERISCOS ES DECIR NO TIENE QUE TENER ESPACIOS AL PRINCIPIO NI AL FINAL**

Usando guiones (-) haces una lista
- Item 1
- Item 2
- Item 3

Tambien podemos poner codigo

```python
print("Hola mundo")
```

Para poner codigo usamos 3 "`" (AltGr + }]) esa tecla

Tambien podemos poner links:


---

## Links

```md id="md5"
[GitHub](https://github.com)


## Comandos para moverse entre carpetas
Usa los mismos comandos que linux
- cd nombre-de-la-carpeta
Si una carpeta tiene espacios
- cd "Nombre de la carpeta"
- cd ..: ir a la carpeta anterior
- cd ~ ó cd: para ir a la carpeta de usuario
- pwd: ver en que carpeta estamos
- ls: ver archivos de la carpta
- ls -la: lo mismo pero con mas detalles



# Comandos Git

- git status: muestra los archivos modificados, que esta listo para el commit y lo que no esta siendo trackeado
- git diff: muestra exactamente que cambio en el codigo
- git add archivo.txt: Agrega un cambio de algun archivo en concreto, ademas prepara para el commit
- git add .: Agrega todos los cambios, ademas prepara para el commit
- git commit -m  "Mensaje": Commit, guarda una version del proyecto
- git log ó git log --oneline: Muestra el historial de commits
- git push: Sube los cambios a GitHub
- git pull: Trae los cambios desde GitHub
- git clone URL: Clona un proyecto
- git log --graph --all

## Comandos de Ramas

- git switch -c nueva-rama: Crea y cambia de rama
- git switch main: Vuelve a la rama principal
- git merge nueva-rama: agrega la rama al main o rama principal
- git branch: Ver en que rama estoy, tambien muestra todas y pone un asterisco en la rama que estoy parado con -r muestra las remotas y con -a muestra todas
- git branch nueva-rama: crea una rama
- git switch nueva-rama: cambia de rama
### Borrar ramas(Importante no estar parado sobre la rama que queremos borrar)
Forma segura si la rama ya esta mergeada a otra rama.
- git branch -d nombre-rama
Si no esta mergeada(la borra aunque cambios sin integrar)
- git branch -D nombre-rama
Si la rama ya esta en GitHub
- git push origin --delete nombre-rama


# ¿Que es una rama?

Es una linea de trabajo independiente dentro del proyecto

Por ejemplo:

main: A --- B --- C
             \
feature:      D --- E

- **Main** es la rama principal del proyecto
- **Feature** es una copia donde probamos cambios sin romper nada

