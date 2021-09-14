## Step 3

Steps to reproduce:

1. Make a new empty directory
2. Create an NPM project in your empty directory

Run in terminal:
```bash
npm init -y
```

package.json:
```json
{
  "name": "temp",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC"
}
```

3. Install Tailwind via NPM

More details and commands can be found here: https://tailwindcss.com/docs/installation#install-tailwind-via-npm

Run in terminal:
```bash
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```

package.json:
```json
{
  "name": "step-3",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "autoprefixer": "^10.3.4",
    "postcss": "^8.3.6",
    "tailwindcss": "^2.2.15"
  }
}
```

4. Install Vite via NPM

More details and commands can be found here: https://tailwindcss.com/docs/guides/vue-3-vite

Run in terminal:
```bash
npm install -D vite
```

```json
{
  "name": "step-3",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "autoprefixer": "^10.3.4",
    "postcss": "^8.3.6",
    "tailwindcss": "^2.2.15",
    "vite": "^2.5.7"
  }
}
```

5. Add a new script in package.json to run vite

```json
{
  "name": "step-3",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "dev": "vite"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "autoprefixer": "^10.3.4",
    "postcss": "^8.3.6",
    "tailwindcss": "^2.2.15",
    "vite": "^2.5.7"
  }
}
```

6. Initialize tailwind and postcss

Run in terminal:
```bash
npx tailwindcss init -p
```

7. Create a index.html file
8. Use emmet to populate default html 5 content

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

9. Create a default TailwindCSS file (for details, go to step 2)

10. Link your new css file in html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="tailwind.css">
</head>
<body>
    
</body>
</html>
```

11. Create an H1 and add some tailwind classes to it

Link to tailwind documentation (starting with Text Color for easy proof of concept) https://tailwindcss.com/docs/text-color

The text-7xl class increases text size, text-red-700 changes text color.

Result:

![image](step-3.PNG)

Complete code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="tailwind.css">
</head>
<body>
    <h1 class="text-7xl text-red-700">Hello World</h1>
</body>
</html>
```