# Tutorial Github By Saepulfariz

## Clone Repo

```CLI
git clone https://github.com/saepulfariz/saepulfariz.github.io.git
```

## Check Remote

```php
git remote
```

```CLI
git remote -v
```

## Check Status

git status

## bikin alias log

alias graph="git log --all --decorate --oneline --graph"
// bisa di panggil graph

## Update

jika untrack add dulu

- git add . <br>
  commit
- git commit -m "menambahkan file index"
- git status maka akan ada hasil mendahului origin master
- git push
- git push --se-upstream origin master

## Revisi GIT

> ### Membatalkan perubahan ( ketika belum git add .)

```CLI
git checkout nama_file.html
```

> ### Membatalkan Perubahan File yang Sudah dalam Kondisi staged
>
> Kondisi staged merupakan kondisi file yang sudah di add (git add), namun belum disimpan (git commit) ke dalam Git.
> git add index.html
> **`git reset index.html`**
> git checkout index.html

## Membatalkan Perubahan File yang Sudah dalam Kondisi Commited

> > git add index.html
> > git commit -m "belajar git greget!"
> > git log
> > buat lihat kode commit
> > git checkout b05f7d05c9298f2cd11b870369f3cf4b2350eca7 index.html
> > git reset index.html
> > Apabila kita ingin mengembalikan seluruh file dalam commit, kita cukup melakukan checkout ke nomer commit saja, tanpa diikuti nama file. Contoh:
> > git checkout ac6d798f98bac5fad693ef8159f957c5b0805c23
> > Catatan: Perintah ini akan mengembalikan semua file dalam kondisi pada nomer commit yang diberikan, namun bersifat temporer.

## Kembali ke 3 Commit sebelumnya

> > git checkout HEAD~3 index.html

## Membatalkan Semua Perubahan yang ada

> > git revert -n <nomer commit>
> > git revert -n 2400ba0e258bd6a144caa273012b130d6baa5e42

## Referensi

- https://www.petanikode.com/git-revert/
- https://www.petanikode.com/git-checkout-reset-revert/

## Buat repo init dengan costum branch

> > git init -b main

## Check Branch

> > git branch

## New branch

git checkout -b ＜ new-branch ＞

## Switching Branches

git checkout ＜ branchname ＞

## Merge branch

> > git branch -M main

## referensi

https://www.atlassian.com/git/tutorials/using-branches/git-checkout#:~:text=The%20git%20branch%20command%20can,to%20switch%20to%20that%20branch.

## Cara buat private repo untuk dari local

> > jangan ceklis Add a README file

## ketika dari local jadi push ke github v2

> > git init
> > git add .
> > git commit -m "Upload File"
> > git remote add origin https://github.com/saepulfariz/git.git
> > git branch -M main
> > git push -u origin main

## ketika dari local jadi push ke github v1

> > git init
> > git remote add origin https://github.com/saepulfariz/git.git
> > git add .
> > git commit - m "upload project"
> > git push

## referensi

https://colamen.id/membuat-github-repository-dari-existing-local-repository/
git push -u origin master
https://stackoverflow.com/questions/23401652/fatal-the-current-branch-master-has-no-upstream-branch
https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github

// buat update
git pull
// jika harus login lagi
git config --list
// keluar denga :q
// --local
git config --global user.name "saepulfariz"
git config --global user.email "saepulfariz108@gmail.com"
// text editor
git config --global core.editor "code -w"

## referensi

https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-config#:~:text=The%20git%
20config%20command%20is,modify%20a%20configuration%20text%20file.
