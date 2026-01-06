# shopify-swatches
The purpose is to select a Shopify collection, use each product’s thumbnail image, and display those images as 50px x 50px swatches on products that are tagged to reference that collection.


### Installation Instructions

## 1) Code Snippet
**Add the snippet to your theme.** <br>
Step 1. Online Store → Themes → Edit code → Snippets → Add new snippet<br>
Step 2. Name it: jaeitee-swatches.liquid<br>
Step 3. Paste code from jaeitee-swatches.liquid<br>

## 2) Create CSS File
Step 1. Online Store → Themes → Edit code → Assets → Add a new asset<br>
Step 2. Name: jaeitee-swatches.css<br>
Step 3. Paste code from jaeitee-swatches.css<br>

## 3) Load CSS File
Step 1. Open Layout → theme.liquid<br>
Step 2. Find <head> secion.<br>
Step 3. Add code near other stylesheets.<br>
{{ 'jaeitee-swatches.css' | asset_url | stylesheet_tag }}<br>

## 4) Insert it on the Product Page
For this you have two options.
