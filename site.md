<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>105x57 Product Card</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Etna', 'Segoe UI', Arial, sans-serif;
    }

    body {
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      background: #f0f4f8;
    }

    .product-card {
      width: 105mm;
      /* bredden på kortet */
      height: 57mm;
      /* höjden på kortet */
      background: #ffffff;
      border-radius: 4mm;
      box-shadow: 0 2mm 5mm rgba(0, 0, 0, 0.1);
      padding: 4mm;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .header {
      background: linear-gradient(135deg, #459bf1, #b6d6f0);
      color: white;
      padding: 4mm 4mm;
      border-radius: 3mm;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 4.5mm;
      font-weight: 600;
      margin: 0.5mm;
    }

    .badge {
      background: #ffffff;
      color: #1976d2;
      padding: 1mm 2.5mm;
      /* main badge, eller kortet som tar störst plats */
      border-radius: 2mm;
      font-size: 3mm;
      font-weight: bold;
      margin-right: 3mm;
      box-shadow: 0 0.5mm 2mm rgba(0, 0, 0, 0.15);
    }

    .brand-model {
      display: inline-block;
    }

    .price {
      font-size: 5mm;
      font-weight: bold;
    }


    .name-block {
      min-height: 16%;
      padding: 4mm;
      margin: 1mm;
      background: #212121;
      border-radius: 4mm;
      color: #ffffff;
      padding: 1mm;
      margin: 0.5mm;
      align-content: center;
      overflow: hidden;
      white-space: nowrap;
      text-overflow: ellipsis;
    }

    /*.description-block {
      min-height: 20%mm;
      background: slategrey;
      color: #424242;
    } */
  
    .footer {
      display: flex;
      align-items: center;
      gap: 4mm;
      margin-top: 3mm;
    }

    .logo-container {
      width: 20%;
      height: 40%;
      margin: 2mm;
      border-radius: 3mm;
      overflow: hidden;
      background: #ffffff;
      box-shadow: 0 0.5mm 2mm rgba(0, 0, 0, 0.15);
      display: flex;
      align-items: center;
      justify-content: center;
      border: 4px solid #ccc;
    }

    .barcode-container {
      flex-grow: 1;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }

    .barcode {
      width: 100%;
      height: 25%;
      margin: 3mm;
      background: #eeeeee;
      display: flex;
      font-size: 3mm;
      color: #9e9e9e;
    }

    .code {
      font-size: 3mm;
      color: #616161;
      margin: 1mm;
    }
  </style>
</head>

<body>

  <div class="product-card">
    <div class="header">
      <div>
        <span class="badge">Nyhet!</span>
        <span class="brand-model">[BRAND] [MODEL]</span>
      </div>
      <div class="price">[PRICE_INC_VAT]</div>
    </div>
    <div class="name-block">
      <span class="block-text">[NAME]</span>
    </div>
    <div class="name-block">
      <span class="block-text">[DESCRIPTION]</span>
    </div>
    <div class="footer">
      <div class="logo-container">
        [IMG_LOGO]
      </div>
      <div class="barcode-container">
        <div class="barcode">[BAR_CODE]</div>
        <div class="code">[CODE]</div>
      </div>
    </div>
  </div>

</body>

</html>
