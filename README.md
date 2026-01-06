# shopify-swatches
The purpose is to select a Shopify collection, use each product’s thumbnail image, and display those images as 50px x 50px swatches on products that are tagged to reference that collection. <br>
<br>
![Swatch Example](assets/swatch_example.png)  <br>
<br>
👉 If you like this project, follow along at https://jaeitee.xyz for more updates.
<br>
## 📚 How to Use
#### Step 1: Create a collection for example called Tasty Apples.<br>
The URL handle for this at the bottom of the page will display tasty-apples.<br>
![Tasty Apples URL Handle](assets/tasty_apples.png)<br>
Add your products to this collection manually.<br>
You can also create a smart collection based on conditions, and this will also work.<br>

#### Step 2: Tag your Products
Add the tag **swatch-tasty-apples** to the products within that collection.<br>
![Tasty Apples TAG](assets/tasty_apples_tag.png)<br>
Any tagged product will now display that swatch.<br>

#### Small Tips
This can work with all your existing collections, just look at your existing URL handles to know the swatch-<url_handle> tag.<br>
Customise the CSS to suit your style, change the active border colour etc.<br>



## 💾 Installation Instructions

### 1) Code Snippet
**Add the snippet to your theme.** <br>
Step 1. Online Store → Themes → Edit code → Snippets → Add new snippet<br>
Step 2. Name it: jaeitee-swatches.liquid<br>
Step 3. Paste code from jaeitee-swatches.liquid<br>

### 2) Create CSS File
Step 1. Online Store → Themes → Edit code → Assets → Add a new asset<br>
Step 2. Name: jaeitee-swatches.css<br>
Step 3. Paste code from jaeitee-swatches.css<br>

### 3) Load CSS File
Step 1. Open Layout → theme.liquid<br>
Step 2. Find <head> secion.<br>
Step 3. Add code near other stylesheets.<br>
<pre>{{ 'jaeitee-swatches.css' | asset_url | stylesheet_tag }}</pre>

### 4) Insert it on the Product Page
For this you have two options.  You can either add custom liquid code inside your theme editor, or continue to edit the code in the code editor.
<br>
**Theme Editor Option**<br>
Step 1: Go to Online Store -> Themes -> Edit Theme<br>
Step 2: Open a Product Page<br>
Step 3: Add a custom liquid code snippet<br>
Step 4: Enter the following code where you want it to appear<br>
<pre>{% render 'jaeitee-swatches' %}</pre>

**Code Edit Option**<br>
Step 1: Go to Online Store -> Themes -> Edit Code<br>
Step 2: Open sections/main-product.liquid<br>
Step 3: Locate where the Price output is.<br>
Step 4: Enter the following code:<br>
<pre>{% render 'jaeitee-swatches' %}</pre>
