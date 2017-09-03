Instructions for adding a new icon tag to the collection:

  - find and save icon to `images/lang/icons/`
  - resize icon: `sips -Z 100 images/lang/icons/TAG`
  - **replace `TAG` variable** to add icon to devved-lang.css 
  - push this repo to github

```css
tag="TEST"; echo -e "\n\n.lang-${tag} {\ndisplay: block;\nbackground: url(https://github.com/devvedNET/blog-assets/blob/master/images/lang/icons/${tag}.png?raw=true);\n}" >> /var/www/html/wp-content/themes/twentyseventeen/devved-lang.css
```