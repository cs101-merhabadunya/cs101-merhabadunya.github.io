# cs101-website

## :memo:To-do 
- [x] Anasayfa
- [x] Kaynaklar
    - [x] Syllabus - Gül Sena
    - [x] Hakkımızda
        may add some things from the inital Syllabus
    - [x] Python referansı :snake: 
    - [x] Pycharm kurulumu :snake: 
    - [x] Pycharm kullanımı
    - [x] Ed üzerinden çalışmaları yükleme
    - [x] Ed kullanım rehberi
    - [x] Grafikler (sonra eklenecek)
    - [x] FAQ - Gül Sena
- [x] Projeler
    - [x] Grup :family:
    - [x] Self-study :computer:
- [x] Dersler
    Kolt python sitesindeki gibi bir tablo iyi olabilir
$$\def\arraystretch{0.8} \begin{array}{llll} Konu & Tarih & Slaytlar & Video \end{array}$$
- [x] Ödevler (ilk ödevden sonra visible olacak)

If it is your first time developing in Jekyll make sure to follow the instructions [here](https://jekyllrb.com/docs/installation/#requirements) based on your operating system.

If this is your first time locally serving this repository execute in the repository folder.
```bundle install```

To view the produced website on your local computer execute the following command:
```bundle exec jekyll serve [--trace --incremental --port XXXX]```

If included `--port XXXX` your server will be directed to `127.0.0.1:XXXX` in the browser. Sometimes using the same port gives error in WSL.

You can find some templates in templates folder, note that the pages inside this folder aren't compiled.
`bundle update` to update all gems to the lates version, `bundle update jekyll` to update jekyll.

Please update the used tags below
- kod
- planlama

## Archiving
When moving up to a next semester, we don't want to delete the older content in the website but archive them. For this purpose we created the `archives` folder. 
- Create the corresponding semester folder in `archives` eg. 2020guz
- Move the contents of `_lectures`, `_posts`, `_projects` and other `.html` files to this folder. Make sure that long term files like about.md, sss.md are still available in the main folder.