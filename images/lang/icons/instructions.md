Instructions for adding a new icon tag to the collection:

  - find and save icon to `images/lang/icons/`
  - resize icon: `sips -Z 100 images/lang/icons/TAG`
  - **replace `TAG_NAME` variable** to add icon to devved-lang.css 

```sh
tag="electron"; echo -e "\n\n.lang-${tag} {\ndisplay: block;\nbackground: url(https://github.com/devvedNET/blog-assets/blob/master/images/lang/icons/${tag}.png?raw=true);\n}" >> /var/www/html/wp-content/themes/twentyseventeen/devved-lang.css
```

  - update local copy of devved-lang.css && push this repo to github
```sh
scp devved:/var/www/html/wp-content/themes/twentyseventeen/devved-lang.css ~/Desktop/devvedNET-root/blog-assets/images/lang/devved-lang.css && git add . && git commit -m 'add lang icons, backup devved-lang css' && git push
```
