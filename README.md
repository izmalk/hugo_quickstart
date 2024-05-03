# Hugo quickstart repo

## Steps to reproduce

0. Install Hugo via: [https://gohugo.io/installation](https://gohugo.io/installation/).  If you have not done so, you will need to download Git, Go and Dart Sass (instructions in the links above).

1. Start Hugo project and create folder structure

```bash
hugo new site quickstart
```

2. Navigate into the project

```bash
cd quickstart
```

3. Initiate submodule and add theme

```bash
git init
git submodule add https://github.com/matcornic/hugo-theme-learn.git themes/learn
```

4. Add the theme to the config:

```bash
echo "theme = 'learn'" >> hugo.toml
```

5. Copy all the files from exampleSite

```bash
cp -R themes/learn/exampleSite/* ./
```

6. Build the web site

```bash
hugo serve
```
