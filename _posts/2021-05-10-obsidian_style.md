
# How to change RTL font in Obsidian

In snippets folder, make a css file like below and add it in the settings.

Note that 'font-face' definition in the beginning is only for learning how to add a font. It's not needed here. because usually we have these fonts in our system fonts.

```css
@font-face {
    /* تعریف نام فونت */
    font-family: 'BZar';
    /* اکسپلورر 9 به بعد */
    src: url('http://example.com/fonts/BZar.eot');
    /* بررسی نصب بودن فونت در سیستم کاربر */
    src: local('bZar'),
         /* برای برخی از مرورگرها مانند سافاری */
         local('b Zar'),
         /* هک برای اکسپلورر 8 و ماقبل */
         url('http://example.com/fonts/BZar.eot?#iefix') format('embedded-opentype'),
         /* فرمت مناسب مرورگرهای خیلی جدید */
         url('http://example.com/fonts/BZar.woff2') format('woff2'),
         /* فرمت مناسب مرورگرهای تقریبا جدید */
         url('http://example.com/fonts/BZar.woff') format('woff'),
         /* تمام مرورگرها به جزء اکسپلورر */
         url('http://example.com/fonts/BZar.ttf') format('truetype'),
         /* نسخه های قدیمی سیستم عامل iOS */
         url('http://example.com/fonts/BZar.svg#BZar') format('svg');
    font-style: normal;
    font-weight: normal;
    font-display: swap;
}






:root {
  --farsi-font-header: 'B Yekan Regular';
  --farsi-font-text:'Vazir';
  
  --default-font: 'Inter',var(--farsi-font-text), -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Microsoft YaHei Light", sans-serif;
  --mermaid-font: var(--default-font);
  --reveal-font: var(--default-font);
  --font-monospace: 'Source Code Pro', monospace;
  
  
}




h1 { font-family: 'Inter',var(--farsi-font-header);}

h2 { font-family: 'Inter',var(--farsi-font-header);}

h3 { font-family: 'Inter',var(--farsi-font-header);}

h4 { font-family: 'Inter',var(--farsi-font-header);}

h5 { font-family: 'Inter',var(--farsi-font-header);}


/*
.markdown-preview-view h1 {
    font-family: inter;
    font-weight: 700 !important;
    font-size: 24px;
    font-weight: normal;
}
*/


```
