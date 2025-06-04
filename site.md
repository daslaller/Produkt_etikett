<invalidtag charset="UTF-8">
  <invalidtag content="width=device-width, initial-scale=1.0" name="viewport">
    <title></title>
    <style type="text/css">
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
        border-radius: 3mm;
        box-shadow: 0 2mm 5mm rgba(0, 0, 0, 0.1);
        padding: 3mm;
        display: flex;
        flex-direction: column;
        gap: 1mm;
        justify-content: space-between;
      }

      .header {
        background: linear-gradient(135deg, #4c9ce6, #174f93);
        color: white;
        min-height: 35%;
        padding: 2mm 2mm 2mm 2mm;
        border-radius: 2.5mm;
        justify-content: space-between;
        display: grid;
        grid-template-columns: repeat(2, min-content);
        grid-template-rows: repeat(2, 1fr);
        grid-column-gap: 0px;
        grid-row-gap: 0px;
        gap: 1mm;
      }

      .badge {
        text-wrap: nowrap;
        background: #ffffff;
        color: #1976d2;
        padding: 1mm 2.5mm;
        /* main badge, eller kortet som tar störst plats */
        border-radius: 2mm;
        font-size: 3mm;
        box-shadow: 0 0.5mm 2mm rgba(0, 0, 0, 0.15);
        grid-area: 1 / 1 / 2 / 2; 
      }

      .pris {
        font-size: 4mm;
        text-align: right;
        grid-area: 1 / 2 / 2 / 3; 
      }

      .namn {
        font-size: 4mm;
        grid-area: 2 / 1 / 3 / 3;
      }

      .name-block {
        min-height: 16%;
        background: #212121;
        border-radius: 3mm;
        color: #ffffff;
        overflow: show;
        align-items: left;
      }

      .block-text {
        padding-left: 3mm;
        font-size: 2.5mm;
        color: #ffffff;
        text-align: left;
        text-overflow: ellipsis;
      }

      /*.description-block { min-height: 20%mm; background: slategrey; color: #424242; } */
      .footer {
        display: flex;
        align-items: center;
        gap: 2mm;
      }

      .logo-container {
        width: 64px;
        height: 64px;
        align-content: center;
        border-radius: 3mm;
        overflow: show;
        background: #ffffff;
        padding: 1mm;
      }

      .barcode-container {
        flex-grow: 1;
        display: flex;
        flex-direction: column;
        align-items: left;
        justify-content: center;
      }

      .barcode {
        width: 100%;
        height: 50%;
        display: flex;
        font-size: 3mm;
        color: #9e9e9e;
      }
    </style>
    <div class="product-card">
      <div class="header">
        <div class="badge">Vi Rekommenderar!</div>

        <div class="pris">[PRICE_INC_VAT]</div>

        <div class="namn">[NAME]</div>
      </div>

      <div class="name-block"><span class="block-text">[MODEL]</span></div>

      <div class="name-block"><span class="block-text">[DESCRIPTION]</span></div>

      <div class="footer">
        <div class="logo-container">[IMG_LOGO]</div>

        <div class="barcode-container">
          <div class="barcode">[BAR_CODE]</div>
        </div>
      </div>
    </div>
  </invalidtag>
</invalidtag>