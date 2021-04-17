# Webslides

## Reference
- [ ] Github repo [here](https://github.com/webslides/WebSlides)

## Steps
1. Create directory structure
- [ ] Create project name at root. Example `Webslides`. 
- [ ] Create `css`, `js`, and `images` directories as child directories to `Webslides`

2. Download Webslides source code from Webslides Github repository
- [ ] Go [here](https://github.com/webslides/WebSlides)
- [ ] Select link for content download

3. Move the source code to your project directory
- [ ] Within the Webslides source code download open the directory labeled `static`
- [ ] Move file `static/css/webslides.css` file to your project `Webslides/css/` directory
- [ ] Move file `static/js/webslides.js` file to your project `Webslides/js/` directory

4. Create boiler plate `html` file
- [ ] Within your project create your `index.html` file with boilerplate html

```html 
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Demo Webslides Project</title>
    </head>
    <body>
    </body>
</html>
```

5. Input `link` and `script` tags required to connect webslides content to `index.html`

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="./css/webslides.css">
        <title>Demo Webslides Project</title>
    </head>
    <body>
        <script src="./js/webslides.js"></script>
    </body>
</html>
```

6. Input the `html` content to contain the slides. Each slide is a `section`.

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./css/webslides.css">
    <title>Demo Webslides Project</title>
</head>

<body>
    <main role="main">
        <article id="webslides" class="horizontal">
            <!-- Slide 1 -->
            <section>
                Slide 1
            </section>
            <!-- Slide 2 -->
            <section>
                Slide 2
            </section>
        </article>
    </main>
    <script src="./js/webslides.js"></script>
</body>
</html>
```

7. Initialize the Webslides javascript object 

```html
    <script src="./js/webslides.js"></script>
    <script>
        window.ws = new WebSlides();
    </script>
```

8. Initate a browser session via `localhost` on port 5500

```javascript
http://127.0.0.1:5500/index.html#slide=1
```

9. Create slides with appropriate styling and tooling. 
- [ ] Nav to here to find appropriate CDN resources [here](https://cdnjs.com/)
- [ ] Utilize the link to find the `font-awesome` and input into the `html` file

```html 
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
        integrity="sha512-iBBXm8fW90+nuLcSKlbmrPcLa0OT92xO1BIsZ+ywDWZCvqsWgccV3gFoRBv0z+8dLJgyAHIhR35VZc2oM/gI1w=="
        crossorigin="anonymous" />
```

- [ ] Input the Google Fonts link from the Github Webslides index.html file into the your `index.html file`

```html 
    <link
        href="https://fonts.googleapis.com/css?family=Roboto:100,100i,300,300i,400,400i,700,700i%7CMaitree:200,300,400,600,700&amp;subset=latin-ext"
        rel="stylesheet">
```