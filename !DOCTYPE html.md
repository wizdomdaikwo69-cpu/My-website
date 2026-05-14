```
<index.html>
<html 
```
```
lang="en">

```
```
<head>
```
```


```
```
  
```
```
<meta charset="UTF-8" />

```
```
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Private Wallet</title>
  <style>
    * {
      margin: 0;
      
```
```
padding: 0;

```
```
      
```
```
box-sizing: border-box;

```
```
      font-family: Arial, sans-serif;
    }

    
```
```
body {

```
```
      
```
```
background: linear-gradient(135deg, #0f172a, #1e293b);

```
```
      display: flex;
      
```
```
justify-content: center;

```
```
      
```
```
align-items: center;

```
```
      
```
```
height: 100vh;

```
```
      color: white;
    }

    
```
```
.card {

```
```
      
```
```
width: 350px;

```
```
      
```
```
background: rgba(255,255,255,0.08);

```
```
      backdrop-filter: blur(10px);
      
```
```
border-radius: 20px;

```
```
      padding: 25px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.3);
      
```
```
text-align: center;

```
```
    }

    
```
```
.profile {

```
```
      
```
```
width: 90px;

```
```
      height: 90px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid white;
      
```
```
margin-bottom: 15px;

```
```
    }

    h2 {
      
```
```
margin-bottom: 10px;

```
```
      font-size: 24px;
    }

    .balance {
      font-size: 36px;
      
```
```
font-weight: bold;

```
```
      margin: 20px 0;
      color: #4ade80;
    }

    
```
```
.small {

```
```
      
```
```
opacity: 0.8;

```
```
      
```
```
margin-bottom: 20px;

```
```
    }

    .btn {
      
```
```
background: #4ade80;

```
```
      color: black;
      
```
```
border: none;

```
```
      
```
```
padding: 12px 20px;

```
```
      
```
```
border-radius: 12px;

```
```
      
```
```
cursor: pointer;

```
```
      font-weight: bold;
      
```
```
transition: 0.3s;

```
```
    }

    
```
```
.btn:hover {

```
```
      
```
```
transform: scale(1.05);

```
```
    }

    
```
```
.edit-box {

```
```
      margin-top: 20px;
      
```
```
text-align: left;

```
```
    }

    
```
```
input {

```
```
      
```
```
width: 100%;

```
```
      padding: 10px;
      
```
```
border-radius: 10px;

```
```
      
```
```
border: none;

```
```
      
```
```
margin-top: 8px;

```
```
      
```
```
margin-bottom: 12px;

```
```
    }
  </style>
</head>
```
```


```
```
<body>

  
```
```
<div class="card">

```
```
    <img
      class="profile"
      id="profilePic"
      src="https://i.pravatar.cc/150?img=12"
      alt="profile"
    />

    <h2 id="username">Michael Johnson</h2>

    <div class="small">Private Premium Wallet</div>

    <div class="balance" id="balance">$4,820,450</div>

    
```
```
<button class="btn" onclick="showAlert()">Transfer Funds</button>

```
```

    
```
```
<div class="edit-box">

```
```
      
```
```
<h3>Edit Details</h3>

```
```

      <input type="text" id="nameInput" placeholder="Change Name" />
      
```
```
<input type="text" id="balanceInput" placeholder="Change Balance" />

```
```
      
```
```
<input type="text" id="imageInput" placeholder="Paste Profile Image URL" />

```
```

      <button class="btn" onclick="updateInfo()">Update Page</button>
    </div>
  
```
```
</div>

```
```

  <script>
    function showAlert() {
      alert('Transfer successful!');
    }

    function updateInfo() {
      const newName = document.getElementById('nameInput').value;
      
```
```
const newBalance = document.getElementById('balanceInput').value;

```
```
      const newImage = document.getElementById('imageInput').value;

      
```
```
if (newName) {

```
```
        document.getElementById('username').innerText = newName;
      }

      
```
```
if (newBalance) {

```
```
        document.getElementById(
```
```
'balance').innerText = newBalance;

```
```
      }

      
```
```
if (newImage) {

```
```
        document.getElementById(
```
```
'profilePic').src = newImage;

```
```
      }
    }
  
```
```
</script>

```
```

</body>
```
```


```
```
</html>

```
