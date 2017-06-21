````shell
172-3-200-128:book Alfred$ cd /Users/Alfred/Desktop/book 
172-3-200-128:book Alfred$ git clone https://git.oschina.net/alfred03/book-axyz.git

172-3-200-128:book Alfred$ cd /Users/Alfred/Desktop/book/book-axyz 
172-3-200-128:book-axyz Alfred$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	README.md
	SUMMARY.md
	_book/
	a/
	b/
	c.md

nothing added to commit but untracked files present (use "git add" to track)
172-3-200-128:book-axyz Alfred$ git add .
172-3-200-128:book-axyz Alfred$ 


172-3-200-128:book-axyz Alfred$ git commit -m 'first commit'
[master (root-commit) 5ecb7cc] first commit
 33 files changed, 3460 insertions(+)
 create mode 100644 README.md
 create mode 100644 SUMMARY.md
 create mode 100644 _book/a/a.html
 create mode 100644 _book/b/b.html
 create mode 100644 _book/c.html
 create mode 100644 _book/gitbook/fonts/fontawesome/FontAwesome.otf
 create mode 100644 _book/gitbook/fonts/fontawesome/fontawesome-webfont.eot
 create mode 100644 _book/gitbook/fonts/fontawesome/fontawesome-webfont.svg
 create mode 100644 _book/gitbook/fonts/fontawesome/fontawesome-webfont.ttf
 create mode 100644 _book/gitbook/fonts/fontawesome/fontawesome-webfont.woff
 create mode 100644 _book/gitbook/fonts/fontawesome/fontawesome-webfont.woff2
 create mode 100644 _book/gitbook/gitbook-plugin-fontsettings/fontsettings.js
 create mode 100644 _book/gitbook/gitbook-plugin-fontsettings/website.css
 create mode 100644 _book/gitbook/gitbook-plugin-highlight/ebook.css
 create mode 100644 _book/gitbook/gitbook-plugin-highlight/website.css
 create mode 100644 _book/gitbook/gitbook-plugin-livereload/plugin.js
 create mode 100644 _book/gitbook/gitbook-plugin-lunr/lunr.min.js
 create mode 100644 _book/gitbook/gitbook-plugin-lunr/search-lunr.js
 create mode 100644 _book/gitbook/gitbook-plugin-search/lunr.min.js
 create mode 100644 _book/gitbook/gitbook-plugin-search/search-engine.js
 create mode 100644 _book/gitbook/gitbook-plugin-search/search.css
 create mode 100644 _book/gitbook/gitbook-plugin-search/search.js
 create mode 100644 _book/gitbook/gitbook-plugin-sharing/buttons.js
 create mode 100644 _book/gitbook/gitbook.js
 create mode 100644 _book/gitbook/images/apple-touch-icon-precomposed-152.png
 create mode 100644 _book/gitbook/images/favicon.ico
 create mode 100644 _book/gitbook/style.css
 create mode 100644 _book/gitbook/theme.js
 create mode 100644 _book/index.html
 create mode 100644 _book/search_index.json
 create mode 100644 a/a.md
 create mode 100644 b/b.md
 create mode 100644 c.md
172-3-200-128:book-axyz Alfred$ git push -u origin master
Counting objects: 49, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (38/38), done.
Writing objects: 100% (49/49), 626.76 KiB | 0 bytes/s, done.
Total 49 (delta 4), reused 0 (delta 0)
To https://git.oschina.net/alfred03/book-axyz.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
172-3-200-128:book-axyz Alfred$ 
````







Setting - Options - Rename可以重命名

