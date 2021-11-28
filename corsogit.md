### inizializzazione
git init

### attuale stato dei files del progetto
git status

### aggiungere files
git add . (tutti i files)
git add file... filen (per aggiungere files separati)
git add *.estensione (solo per alcune estensioni)

### creare commit
git commit -m "*commento*

### scartare le modifiche
git restore *file* (o .)

### rimuovere dalla staging area un file
git restore --staged *file*

### storico delle commit
git log
(ogni commit ha una chiave in sha1, es.: commit 4cb5024169791af4df72b7e655de937b4033deee)

indica anche il branch es.: (HEAD -> master)

git log --reverse (per leggere dal primo commit all'ultima i log)

git log --oneline (per indicare in una riga i commit)

### per verificare il percorso delle nostre commit
git log --all --decorate --graph --oneline

### per modificare l'ultimo commit
git commit --amend

### per indicare a git di non considerare altri files
inserire il file nel file .gitignore
(è possibile anche utilizzare *.estensione)
per creare un'eccezione in gitignore è possibile far procedere il file da !
in questo modo git considererà il file

ad es.: 
*.log
!debug.log

per escludere una cartella basta scrivere la cartella
es.: temp

### creare alias per i comandi
alias *nome*='*comando*'
es.: alias graph='git log --all --decorate --graph --oneline'

### creare nuovi branch
git branch *nomebranch*

### elencare i branch
git branch

### spostarsi tra i branch
git checkout *nomebranch*

## creare e spostarsi in un branch
git checkout -b *nomebranch*

### verificare differenze tra branch
git diff *nomebranch*..*nomebranch*

### unire i branch
git merge *nomebranch* (merge fastforward ad una via)

### eliminare un branch
git -d *nomebranch*

### push in github
git remote add origin https://github.com/sam-sepi/*nome repo*.git

git push https://*token dev*@github.com/sam-sepi/*nome repo*.git

### leggere il file di configurazione
cat .git/config

### informazioni sul server remoto
git remote show *nome server*
es.: git remote show origin

### rinominare server remote
git remote rename *nome* *nuovonome*

### sincronizzare dal remoto al locale
