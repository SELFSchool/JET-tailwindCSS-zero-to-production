## Step 2

Steps to reproduce:

1. Make a new empty directory
2. Create a index.html file
3. Use emmet to populate default html 5 content

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

4. Create default tailwind.css, default contents are: 

```css
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
```

You can find the contents of this file and more information here: https://tailwindcss.com/docs/installation#include-tailwind-in-your-css

For now, you don't really need to worry about what it does.

5. Generate output css using Tailwind CLI

You can find the commands and the output here: https://tailwindcss.com/docs/installation#using-tailwind-cli

Run command:

```bash
npx tailwindcss -o css/style.css
```

6. In your html file, link your new styles.css file.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    
</body>
</html>
```

7. Create an H1 and add some tailwind classes to it

Link to tailwind documentation (starting with Text Color for easy proof of concept) https://tailwindcss.com/docs/text-color

The text-7xl class increases text size, text-red-700 changes text color.

Result:

![image](step-2.PNG)

Complete code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <h1 class="text-7xl text-red-700">Hello World</h1>
</body>
</html>
```