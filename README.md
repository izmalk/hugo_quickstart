# Hugo quickstart repo

## Steps to reproduce

1. Install Hugo (and if necessary Git, Go and Dart Sass): follow instructions in [https://gohugo.io/installation](https://gohugo.io/installation/).
   
2. Start Hugo project and create folder structure

```bash
hugo new site quickstart
```

3. Navigate into the project

```bash
cd quickstart
```

4. Initiate submodule and add theme

```bash
git init
git submodule add https://github.com/matcornic/hugo-theme-learn.git themes/learn
```

5. Add the theme to the config:

```bash
echo "theme = 'learn'" >> hugo.toml
```

6. Copy all the files from exampleSite

```bash
cp -R themes/learn/exampleSite/* ./
```

7. Build the web site

```bash
hugo serve
```
