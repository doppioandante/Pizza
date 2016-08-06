# Compilazione

La compilazione di Pizza richiede 3 semplicissime fasi descritte di seguito.

Paradossalmente la fase piu' complicata e' la preparazione dell'ambiente di lavoro!


## Preparazione

L'installazione del compilatore e runtime java e' necessaria per lavorare con il progetto!

La versione utilizzata al momento della creazione del progetto e': [jdk 1.8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

Il processo di compilazione e' automatizzato da [ant](http://ant.apache.org/bindownload.cgi): e' necessario aggiungere la directory bin alla variabile d'ambiente PATH!

Per scaricare il progetto e' necessario installare [git](https://git-scm.com/) con il plugin [git-lfs](https://git-lfs.github.com/)!


## Ottenere il codice sorgente

L'utilizzo di git e' altamente consigliato per scaricare il codice sorgente:

```sh
git clone https://github.com/NeroReflex/Pizza.git
cd Pizza
```

Ora e' possibile passare alla compilazione vera e propria!


## Compilazione

Il processo di compilazione e' descritto nel file nbbuild.xml, destinato al build system ant,
e va azionato con il comando:

```sh
ant -f nbbuild.xml
```

Una corretta compilazione produrra' una directory "dist" contenente un file chiamato "Pizza.jar",
tuttavia il programma non potra' ancora essere avviato: e' infatti necessario creare una cartella "lib"
allo stesso livello del programma compilato e copiarvi dentro le librerie necessarie che troverete nella root
del progetto!