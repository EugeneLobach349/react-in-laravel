## React and TypeScript in Laravel

## Creating Laravel application:
```shell
laravel new project-name
```
or
```shell
composer create-project laravel/laravel project-name
```

## Installing dependencies:
```shell
npm install react @types/react react-dom react-router-dom  typescript @babel/preset-react ts-loader
```

## Initialise TypeScript:
```shell
tsc --init --jsx react
```

## Change Laravel Mix file to this:
```javascript
mix.ts('resources/js/app.js', 'public/js')
    .postCss('resources/css/app.css', 'public/css', [
        //
    ]).react();
```

## And run your app:
### Laravel:
```shell
php artisan serve
```
### Node.js (Laravel Mix)
```shell
npm run watch
```
for auto compiling after changes

or 
```shell
npm run dev
```
for manual compiling
