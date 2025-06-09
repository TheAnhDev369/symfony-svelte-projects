# symfonysvelte

##  Khởi tao dự Án Symfony (BackEnd) + Svelte (FrontEnd)
```git
git init
echo "# symfonysvelte" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/TheAnhDev369/symfonysvelte.git
git push -u origin main
```

### Cài Symfony project

```php
composer create-project symfony/skeleton my_project
cd my_project
composer require api
composer require symfony/orm-pack symfony/maker-bundle
composer require cors
```

-   symfony/orm-pack → dùng Doctrine ORM (nếu có database)

-   symfony/maker-bundle → giúp tạo code nhanh

-   api → cài API Platform nếu muốn build REST API dễ

-   cors → cho phép frontend Svelte fetch API

### Cài Svelte project (tách riêng folder frontend)

```js
cd ..
npx degit sveltejs/template my_project_frontend
cd my_project_frontend
npm install
```