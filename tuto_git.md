Total in 12 ms
^Cfhc@fhc-pc:~/go/fhc_sitels
archetypes   content  deploy.sh  netlify.toml  resources  themes
config.toml  data     layouts    public        static
fhc@fhc-pc:~/go/fhc_site$ cd content
fhc@fhc-pc:~/go/fhc_site/content$ ls
about  post  posts
fhc@fhc-pc:~/go/fhc_site/content$ cd post
fhc@fhc-pc:~/go/fhc_site/content/post$ ls
first-post.md  my-first-post.md
fhc@fhc-pc:~/go/fhc_site/content/post$ cd ../posts
fhc@fhc-pc:~/go/fhc_site/content/posts$ ls
fhc@fhc-pc:~/go/fhc_site/content/posts$ vim

Command 'vim' not found, but can be installed with:

sudo apt install vim         # version 2:8.1.2269-1ubuntu5, or
sudo apt install vim-tiny    # version 2:8.1.2269-1ubuntu5
sudo apt install neovim      # version 0.4.3-3
sudo apt install vim-athena  # version 2:8.1.2269-1ubuntu5
sudo apt install vim-gtk3    # version 2:8.1.2269-1ubuntu5
sudo apt install vim-nox     # version 2:8.1.2269-1ubuntu5

fhc@fhc-pc:~/go/fhc_site/content/posts$ cd ..
fhc@fhc-pc:~/go/fhc_site/content$ hugo server
Error: Unable to locate config file or config directory. Perhaps you need to create a new site.
       Run `hugo help new` for details.

fhc@fhc-pc:~/go/fhc_site/content$ cd ..
fhc@fhc-pc:~/go/fhc_site$ hugo server
Building sites … WARN 2021/07/06 23:24:06 .File.UniqueID on zero object. Wrap it in if or with: {{ with .File }}{{ .UniqueID }}{{ end }}
WARN 2021/07/06 23:24:06 .File.Path on zero object. Wrap it in if or with: {{ with .File }}{{ .Path }}{{ end }}

                   | EN  
-------------------+-----
  Pages            | 10  
  Paginator pages  |  0  
  Non-page files   |  0  
  Static files     | 59  
  Processed images |  0  
  Aliases          |  1  
  Sitemaps         |  1  
  Cleaned          |  0  

Built in 38 ms
Watching for changes in /home/fhc/go/fhc_site/{archetypes,content,data,layouts,static,themes}
Watching for config changes in /home/fhc/go/fhc_site/config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop

Change detected, rebuilding site.
2021-07-06 23:25:01.709 +0200
Source changed "/home/fhc/go/fhc_site/content/post/first-post.md": RENAME
Source changed "/home/fhc/go/fhc_site/content/posts/first-post.md": CREATE
WARNING: calling IsSet with unsupported type "ptr" (*hugolib.SiteInfo) will always return false.

Total in 10 ms
^Cfhc@fhc-pc:~/go/fhc_site$ hugo server
Building sites … WARN 2021/07/06 23:25:50 .File.UniqueID on zero object. Wrap it in if or with: {{ with .File }}{{ .UniqueID }}{{ end }}
WARN 2021/07/06 23:25:50 .File.Path on zero object. Wrap it in if or with: {{ with .File }}{{ .Path }}{{ end }}
WARNING: calling IsSet with unsupported type "ptr" (*hugolib.SiteInfo) will always return false.


                   | EN  
-------------------+-----
  Pages            | 10  
  Paginator pages  |  0  
  Non-page files   |  0  
  Static files     | 59  
  Processed images |  0  
  Aliases          |  1  
  Sitemaps         |  1  
  Cleaned          |  0  

Built in 36 ms
Watching for changes in /home/fhc/go/fhc_site/{archetypes,content,data,layouts,static,themes}
Watching for config changes in /home/fhc/go/fhc_site/config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop

Change detected, rebuilding site.
2021-07-06 23:28:57.716 +0200
Source changed "/home/fhc/go/fhc_site/content/post": RENAME
WARNING: calling IsSet with unsupported type "ptr" (*hugolib.SiteInfo) will always return false.

Total in 9 ms

Change detected, rebuilding site.
2021-07-06 23:31:09.716 +0200
Source changed "/home/fhc/go/fhc_site/content/posts/first-post.md": CREATE
WARNING: calling IsSet with unsupported type "ptr" (*hugolib.SiteInfo) will always return false.

Total in 5 ms
^Cfhc@fhc-pc:~/go/fhc_site$ git remote add origin https://github.com/fhcomputer/fhcomputer.github.io.git
fhc@fhc-pc:~/go/fhc_site$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   .gitmodules
	new file:   hugo-creative-portfolio-theme
	new file:   themes/cactus

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	deleted:    hugo-creative-portfolio-theme

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	archetypes/
	config.toml
	content/
	data/
	deploy.sh
	netlify.toml
	public/
	resources/
	themes/creative/
	themes/hugo-creative-portfolio-theme/

fhc@fhc-pc:~/go/fhc_site$ git add --all
fhc@fhc-pc:~/go/fhc_site$ git commit -m "Initial commit"
[master (root-commit) 7f22219] Initial commit
 217 files changed, 53016 insertions(+)
 create mode 100644 .gitmodules
 create mode 100644 archetypes/default.md
 create mode 100644 config.toml
 create mode 100644 content/about/index.md
 create mode 100644 content/posts/first-post.md
 create mode 100644 data/projects.json
 create mode 100644 deploy.sh
 create mode 100644 netlify.toml
 create mode 100644 public/404.html
 create mode 100644 public/categories/index.html
 create mode 100644 public/categories/index.xml
 create mode 100644 public/css/bootstrap.min.css
 create mode 100644 public/css/bootstrap.min.css.map
 create mode 100644 public/css/custom.css
 create mode 100644 public/css/font-awesome.min.css
 create mode 100644 public/css/fonts/FontAwesome.otf
 create mode 100644 public/css/fonts/fontawesome-webfont.eot
 create mode 100644 public/css/fonts/fontawesome-webfont.svg
 create mode 100644 public/css/fonts/fontawesome-webfont.ttf
 create mode 100644 public/css/fonts/fontawesome-webfont.woff
 create mode 100644 public/css/fonts/fontawesome-webfont.woff2
 create mode 100644 public/css/helper.css
 create mode 100644 public/css/owl.carousel.css
 create mode 100644 public/css/owl.theme.css
 create mode 100644 public/css/owl.transitions.css
 create mode 100644 public/css/style.blue.css
 create mode 100644 public/css/style.default.css
 create mode 100644 public/css/style.green.css
 create mode 100644 public/css/style.pink.css
 create mode 100644 public/css/style.red.css
 create mode 100644 public/css/style.sea.css
 create mode 100644 public/css/style.violet.css
 create mode 100644 public/fonts/glyphicons-halflings-regular.ttf
 create mode 100644 public/index.html
 create mode 100644 public/index.xml
 create mode 100644 public/js/bootstrap.min.js
 create mode 100644 public/js/ekko-lightbox.js
 create mode 100644 public/js/front.js
 create mode 100644 public/js/imagesloaded.pkgd.min.js
 create mode 100644 public/js/jquery.cookie.js
 create mode 100644 public/js/jquery.min.js
 create mode 100644 public/js/jquery.scrollTo.min.js
 create mode 100644 public/js/masonry.pkgd.min.js
 create mode 100644 public/js/owl.carousel.min.js
 create mode 100644 public/posts/index.html
 create mode 100644 public/posts/index.xml
 create mode 100644 public/posts/my-first-post/index.html
 create mode 100644 public/sitemap.xml
 create mode 100644 public/tags/index.html
 create mode 100644 public/tags/index.xml
 create mode 100644 resources/_gen/assets/scss/scss/style.scss_17a317b87063135b4df76ed814d78726.content
 create mode 100644 resources/_gen/assets/scss/scss/style.scss_17a317b87063135b4df76ed814d78726.json
 create mode 160000 themes/cactus
 create mode 100644 themes/creative/LICENSE
 create mode 100644 themes/creative/README.md
 create mode 100644 themes/creative/archetypes/default.md
 create mode 100644 themes/creative/archetypes/portfolio.md
 create mode 100644 themes/creative/exampleSite/config.toml
 create mode 100644 themes/creative/exampleSite/content/about/_index.md
 create mode 100644 themes/creative/exampleSite/content/contact/_index.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work1.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work10.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work11.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work2.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work3.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work4.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work5.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work6.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work7.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work8.md
 create mode 100644 themes/creative/exampleSite/content/portfolio/work9.md
 create mode 100644 themes/creative/exampleSite/static/img/about.jpg
 create mode 100644 themes/creative/exampleSite/static/img/favicon.png
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/a4-paper.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/business-card-26.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/business-card.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/envelope-brand.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/gravity-paper.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/ipad-air-2.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/label-clothes.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/paper-presentation.jpg
 create mode 100644 themes/creative/exampleSite/static/img/portfolio/trifold.jpg
 create mode 100644 themes/creative/images/screenshot.png
 create mode 100644 themes/creative/images/tn.png
 create mode 100644 themes/creative/layouts/404.html
 create mode 100644 themes/creative/layouts/_analytics/matomo.html
 create mode 100644 themes/creative/layouts/_default/baseof.html
 create mode 100644 themes/creative/layouts/_default/list.html
 create mode 100644 themes/creative/layouts/_default/single.html
 create mode 100644 themes/creative/layouts/about/list.html
 create mode 100644 themes/creative/layouts/contact/list.html
 create mode 100644 themes/creative/layouts/index.html
 create mode 100644 themes/creative/layouts/partials/attribution.html
 create mode 100644 themes/creative/layouts/partials/footer.html
 create mode 100644 themes/creative/layouts/partials/head.html
 create mode 100644 themes/creative/layouts/partials/header.html
 create mode 100644 themes/creative/layouts/partials/mobile_nav_toggle.html
 create mode 100644 themes/creative/layouts/partials/portfolio.html
 create mode 100644 themes/creative/layouts/partials/scripts.html
 create mode 100644 themes/creative/layouts/partials/sidebar.html
 create mode 100644 themes/creative/layouts/partials/social_buttons_in_contact.html
 create mode 100644 themes/creative/layouts/partials/social_buttons_in_sidebar.html
 create mode 100644 themes/creative/static/css/bootstrap.min.css
 create mode 100644 themes/creative/static/css/bootstrap.min.css.map
 create mode 100644 themes/creative/static/css/custom.css
 create mode 100644 themes/creative/static/css/font-awesome.min.css
 create mode 100644 themes/creative/static/css/fonts/FontAwesome.otf
 create mode 100644 themes/creative/static/css/fonts/fontawesome-webfont.eot
 create mode 100644 themes/creative/static/css/fonts/fontawesome-webfont.svg
 create mode 100644 themes/creative/static/css/fonts/fontawesome-webfont.ttf
 create mode 100644 themes/creative/static/css/fonts/fontawesome-webfont.woff
 create mode 100644 themes/creative/static/css/fonts/fontawesome-webfont.woff2
 create mode 100644 themes/creative/static/css/helper.css
 create mode 100644 themes/creative/static/css/owl.carousel.css
 create mode 100644 themes/creative/static/css/owl.theme.css
 create mode 100644 themes/creative/static/css/owl.transitions.css
 create mode 100644 themes/creative/static/css/style.blue.css
 create mode 100644 themes/creative/static/css/style.default.css
 create mode 100644 themes/creative/static/css/style.green.css
 create mode 100644 themes/creative/static/css/style.pink.css
 create mode 100644 themes/creative/static/css/style.red.css
 create mode 100644 themes/creative/static/css/style.sea.css
 create mode 100644 themes/creative/static/css/style.violet.css
 create mode 100644 themes/creative/static/fonts/glyphicons-halflings-regular.ttf
 create mode 100644 themes/creative/static/js/bootstrap.min.js
 create mode 100644 themes/creative/static/js/ekko-lightbox.js
 create mode 100644 themes/creative/static/js/front.js
 create mode 100644 themes/creative/static/js/imagesloaded.pkgd.min.js
 create mode 100644 themes/creative/static/js/jquery.cookie.js
 create mode 100644 themes/creative/static/js/jquery.min.js
 create mode 100644 themes/creative/static/js/jquery.scrollTo.min.js
 create mode 100644 themes/creative/static/js/masonry.pkgd.min.js
 create mode 100644 themes/creative/static/js/owl.carousel.min.js
 create mode 100644 themes/creative/theme.toml
 create mode 100644 themes/hugo-creative-portfolio-theme/.gitignore
 create mode 100644 themes/hugo-creative-portfolio-theme/.travis.yml
 create mode 100644 themes/hugo-creative-portfolio-theme/LICENSE
 create mode 100644 themes/hugo-creative-portfolio-theme/README.md
 create mode 100644 themes/hugo-creative-portfolio-theme/archetypes/default.md
 create mode 100644 themes/hugo-creative-portfolio-theme/archetypes/portfolio.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/config.toml
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/about/_index.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/contact/_index.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work1.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work10.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work11.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work2.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work3.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work4.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work5.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work6.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work7.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work8.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/content/portfolio/work9.md
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/about.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/favicon.png
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/a4-paper.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/business-card-26.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/business-card.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/envelope-brand.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/gravity-paper.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/ipad-air-2.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/label-clothes.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/paper-presentation.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/exampleSite/static/img/portfolio/trifold.jpg
 create mode 100644 themes/hugo-creative-portfolio-theme/images/screenshot.png
 create mode 100644 themes/hugo-creative-portfolio-theme/images/tn.png
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/404.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/_analytics/matomo.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/_default/baseof.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/_default/list.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/_default/single.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/about/list.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/contact/list.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/index.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/attribution.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/footer.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/head.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/header.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/mobile_nav_toggle.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/portfolio.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/scripts.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/sidebar.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/social_buttons_in_contact.html
 create mode 100644 themes/hugo-creative-portfolio-theme/layouts/partials/social_buttons_in_sidebar.html
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/bootstrap.min.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/bootstrap.min.css.map
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/custom.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/font-awesome.min.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/fonts/FontAwesome.otf
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/fonts/fontawesome-webfont.eot
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/fonts/fontawesome-webfont.svg
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/fonts/fontawesome-webfont.ttf
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/fonts/fontawesome-webfont.woff
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/fonts/fontawesome-webfont.woff2
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/helper.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/owl.carousel.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/owl.theme.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/owl.transitions.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/style.blue.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/style.default.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/style.green.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/style.pink.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/style.red.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/style.sea.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/css/style.violet.css
 create mode 100644 themes/hugo-creative-portfolio-theme/static/fonts/glyphicons-halflings-regular.ttf
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/bootstrap.min.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/ekko-lightbox.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/front.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/imagesloaded.pkgd.min.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/jquery.cookie.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/jquery.min.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/jquery.scrollTo.min.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/masonry.pkgd.min.js
 create mode 100644 themes/hugo-creative-portfolio-theme/static/js/owl.carousel.min.js
 create mode 100644 themes/hugo-creative-portfolio-theme/theme.toml
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ 
fhc@fhc-pc:~/go/fhc_site$ git push -u origin master
Username for 'https://github.com': ^C
fhc@fhc-pc:~/go/fhc_site$ git push -u origin fhc_site
error: src refspec fhc_site does not match any
error: failed to push some refs to 'https://github.com/fhcomputer/fhcomputer.github.io.git'
fhc@fhc-pc:~/go/fhc_site$ git push -u origin master
Username for 'https://github.com': fhcomputer
Password for 'https://fhcomputer@github.com': 
Enumerating objects: 146, done.
Counting objects: 100% (146/146), done.
Delta compression using up to 4 threads
Compressing objects: 100% (127/127), done.
Writing objects: 100% (146/146), 1.85 MiB | 3.33 MiB/s, done.
Total 146 (delta 25), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (25/25), done.
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/fhcomputer/fhcomputer.github.io/pull/new/master
remote: 
To https://github.com/fhcomputer/fhcomputer.github.io.git
 * [new branch]      master -> master
Branch 'master