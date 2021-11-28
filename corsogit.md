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

### rimuovere dalla staging area un file
git restore --staged *file*

### storico delle commit
git log
(ogni commit ha una chiave in sha1, es.: commit 4cb5024169791af4df72b7e655de937b4033deee)

indica anche il branch es.: (HEAD -> master)

git log --reverse (per leggere dal primo commit all'ultima i log)

### per modificare l'ultimo commit
git commit --amend

### per indicare a git di non considerare altri files
inserire il file nel file .gitignore
(è possibile anche utilizzare *.estensione)