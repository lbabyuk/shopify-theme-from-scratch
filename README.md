[HW]  Minimal theme from scratch (without schema), with a connected educational section

###  Task description
Create a working theme framework from scratch (OS 2.0) in Liquid:
- A basic layout/theme.liquid layout with content_for_header and content_for_layout.  
- Connect your educational section (from the previous lesson) in the appropriate template. 
- Break repeated code into snippets.Break repeated code into snippets. 
- Move all texts into translations using t.
-   
#### Constraints and Requirements:
- No schema in sections at this stage.
- Header and footer must be sections.
- All repeated HTML (cards, buttons, navigation) must go into snippets, included via render.
- All functional/service texts must use t (locales in locales/*.json).
- No include — use only render.
- Clean HTML: use {%- … -%} to control whitespace, meaningful alt attributes, proper semantics and ARIA roles.
- System links must come only from routes.

### Features Implemented
1. Implemented a minimal folder structure for the Shopify theme (OS 2.0) with separate directories for layout, sections, snippets, assets, and locales.
2. Created basic layout/theme.liquid with content_for_header and content_for_layout;
3. Created banner product cart snippet in **snippets/banner-product.liquid**;
4.  Breaks the product card snippet  into reusable **sub-snippets** using **`render`**:
    - banner-product-add-to-cart.liquid,
    - banner-product-color.liquid,
    - banner-product-shoe-size.liquid, 
    - banner-product-price.liquid,
    - banner-product-not-found.liquid.
    - logo.liquid.
    - nav-main.liquid.
5. Texts localized with **t** and fallback;
6. For features implementations created for JS:  in assets folder **banner-product-cart.js** file, for CSS - **panner-product.css**, **base.css**;
7. Created sections in sections/ : footer.liquid, header.liquid, product.liquid;
8. Created locales in locales/uk.defaulte.json;      

### Related links:
1. [Asana note](https://app.asana.com/1/442123638460530/project/1211341031891215/task/1211341863851843?focus=true)
2. [Theme preview](https://dawn-ob.myshopify.com/?preview_theme_id=187671773522)
**Password**:  debree1234
