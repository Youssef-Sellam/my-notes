
## Comandi di base delle cartelle

### clear
Il comando `clear` pulisce la shell in cui stai lavorando.

### ls
Il comando `ls` serve per vedere il nome delle cartelle che si hanno. Se si aggiunge `/`, si possono vedere le cartelle di una precisa directory. Se si aggiunge `-a`, mostra anche le directory nascoste.

#### Esempi `ls`
```bash
sysadmin@localhost:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos

sysadmin@localhost:~$ ls -a
.            .bashrc   .selected_editor  Downloads  Public
..            .cache    Desktop           Music      Templates
.bash_logout  .profile  Documents         Pictures   Videos

sysadmin@localhost:~$ ls -l /var/log/
total 900
-rw-r--r-- 1 root   root  15322 Dec 10 21:33 alternatives.log
-rw-r----- 1 syslog adm     371 Dec 15 16:38 auth.log
-rw-rw---- 1 root   utmp      0 May 26  2018 btmp
-rw-r--r-- 1 root   adm   85083 Dec 10 21:33 dmesg
-rw-r--r-- 1 root   root  32064 Dec 10 21:33 faillog
-rw-rw-r-- 1 root   utmp 292584 Dec 15 16:38 lastlog
-rw------- 1 root   root  64128 Dec 10 21:33 tallylog
#### Tipi di file

|Simbolo|Tipo di file|Descrizione|
|---|---|---|
|`d`|directory|Un file utilizzato per archiviare altri file.|
|`l`|link simbolico|Punta a un altro file.|
|`p`|pipe|Permette la comunicazione tra processi.|
|`c`|file di caratteri|Un file di dispositivo a caratteri.|

### pwd

Il comando `pwd` serve a vedere il percorso delle directory in cui sei ora.

### cd

Il comando `cd` è la abbreviazione di "change directory", infatti come dice il nome ti fa cambiare la directory corrente. Non puoi mettere nomi a caso perché ti dà errore.

#### Esempi `cd` e `pwd`

```
# Per entrare in una directory
sysadmin@localhost:~/Documents$ cd School/Art
sysadmin@localhost:~/Documents/School/Art$

# Per vedere il percorso di una directory
sysadmin@localhost:~/Documents/School/Art$ pwd
/home/sysadmin/Documents/School/Art

# Per uscire da una directory
sysadmin@localhost:~/Documents/School/Art$ cd ..
sysadmin@localhost:~/Documents/School$ pwd
/home/sysadmin/Documents/School
```

## Altri comandi utili

### mkdir

Il comando `mkdir` serve per creare una nuova directory.

```
mkdir nome_della_directory
```

### rm

Il comando `rm` serve per rimuovere file o directory.
```
# Per rimuovere un file
rm nome_del_file

# Per rimuovere una directory
rm -r nome_della_directory
```

### touch

Il comando `touch` serve per creare un nuovo file vuoto.

```
touch nome_del_file
```

### cp

Il comando `cp` serve per copiare file o directory.

```
# Per copiare un file

### cp

Il comando `cp` serve per copiare file o directory.

bash

```
# Per copiare un file
cp nome_file_originale nome_file_destinazione

# Per copiare una directory
cp -r nome_directory_originale nome_directory_destinazione
```

### mv

Il comando `mv` serve per spostare o rinominare file o directory.

bash

```
# Per spostare un file
```
### echo

Il comando `echo` serve per visualizzare messaggi o variabili.

bash

```
echo "Ciao, mondo!"
```

