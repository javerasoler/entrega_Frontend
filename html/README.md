# html exercises

In this exercises you will have to complete the missing html or remark what should we include. For example:

What is wrong with this HTML?

```html
<customtag>lorem ipsum dolor</customtab>
```

Answer: It is using a key that does not exists.

## Exercise 1

Add what is missing in our html `<head>` tag.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Document</title>
  </head>
</html>
```

Answer: Falta una línea con <meta charset="UTF-8"> arriba <title>


## Exercise 2

This html is not semantic what could we do to improve it.

```html
<div class="main">
  <div class="section">
    <div>
      <div class="list-item">List item</div>
      <div class="list-item">List item</div>
      <div class="list-item">List item</div>
      <div class="list-item">List item</div>
    </div>
  </div>
  <div class="section">
    <div class="form">
      <label>description</label>
      <input type="text">
    </div>
  </div>
</div>
```html

Answer: 

<body class="main">
  <section class="section">
    <ul>
      <li class="list-item">List item</li>
      <li class="list-item">List item</li>
      <li class="list-item">List item</li>
      <li class="list-item">List item</li>
    </ul>
  </section>
  <section class="section">
    <form class="form">
      <label>description</label>
      <input type="text">
    </form>
  </section>
</body>


## Exercise 3

If we want to include two CSS files like `reset.css`, `main.css`, and one javascript file `app.js`. Where should we include it in this html?

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
Answer: 

  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <link rel="stylesheet" href="reset.css">
  <link rel="stylesheet" href="main.css">
</head>
<body>
.
.
.(al final)
<script src="dist/main.js"></script>
</body>
</html>
```

## Exercise 4

We need to improve this html form markup. This form will call and endpoint `/register` with the right method. We also have to include the correct input type and mark all fields as required.

```html
<form>
  <div>
    <label>name</label>
    <input type="text" id="name" name="name" required>
  </div>
  <div>
    <label>surname</label>
    <input type="text" id="surname" name="surname"> required>
  </div>
  <div>
    <label>phone</label>
    <input type="tel" id="phone" name="phone"> 
  </div>
  <div>
    <label>email</label>
    <input type="email" id="userEmail" name="userEmail"> 
  </div>
  <div>
    <label>password</label>
    <input type="password" id="userPwd" name="password"> 
  </div>
  <input value="register">
</form>
```

Answer: action method