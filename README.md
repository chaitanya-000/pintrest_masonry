![README banner with text](https://github.com/chaitanya-000/pintrest_masonry/assets/103093624/0d943ce1-b1dc-438a-9d4e-d50e21befb1e)

Pintrest Masonry with HTML & CSS

Create Pintrest like Masonry with just HTML & CSS. Copy-paste and customize. 


CSS
* {
  margin: 0;
  box-sizing: border-box;
  overflow-x: hidden;  // It essentially prevents horizontal scrolling.
}

.container {
  width: 100%;
  margin: 10px auto;  //Adds vertical margin
  columns: 5;   //Changes the number of columns. 
  column-gap: 1vh;  //Increases the space between columns. 
  padding: 1%; 
}
.container .box {
  width: 100%;
  border-radius: 10px;
}

.container .box img {
  max-width: 100%;
}

@media (0 < width < 768px) {
  .container {
    columns: 2;  //For mobiles, we keep two columns
    padding: 2%;  //Keep the padding more for better spacing. 
  }
}
@media (769px < width < 1279px) {
  .container {
    columns: 3;  //For Tablets, we keep three columns
    padding: 2%;
  }
}
