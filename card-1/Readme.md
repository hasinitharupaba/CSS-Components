# HTML Code

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Card component by Paba Codes</title>
  <link rel="stylesheet" href="/styles.css" />
</head>
<body>
  <div class="card">
    <h1>Card</h1>
  </div>
</body>
</html>

```

# CSS styles

```
* {
  font-family:Arial, Helvetica, sans-serif
}

body{
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.card {
  width: 200px;
  height: 260px;
  background: black;
  position: relative;
  display: flex;
  place-content: center;
  place-items: center;
  overflow: hidden;
  border-radius: 12px;
}

.card h1 {
  color: white;
  z-index: 1;
  font-size: 2rem;
  text-transform: uppercase;
}

.card::before{
  content: '';
  position: absolute;
  width: 160px;
  background-image: linear-gradient(90deg, #CB4DEB, #F9F254 );
  height: 140%;
  animation: rotateBgImg 5s linear infinite;
  transition: all 0.3s linear;
}

@keyframes rotateBgImg {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  }
}

.card::after{
  content: '';
  position: absolute;
  background: black;
  inset: 4px;
  border-radius: 12px;
}
```
