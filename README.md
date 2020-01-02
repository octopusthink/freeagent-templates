# FreeAgent Invoice Devkit

From: http://www.freeagent.com/support/kb/invoicing/css-guide-for-invoice-templates/

-----

## Edit your CSS
Duplicate both screen and print CSS files for whatever theme you want to base yours on and rename them (or simply create your own from scratch, but be aware this will be much harder). Now change the stylesheet paths in `index.html` to reference your new stylesheets.

Make all of the changes to your theme CSS. Remember that your invoice has to render well as a PDF in addition to the on-screen preview. Theme layouts also change depending on what state they’re in (e.g. a draft invoice has additional elements like the "Add Invoice Item" button), and when other company-type content is present (e.g. a sales tax column).

When you’re happy with your changes and want to test them, paste your CSS into the custom theme area of your FreeAgent account. Our [guide to creating custom invoice themes](http://www.freeagent.com/support/kb/invoicing/css-guide-for-invoice-templates/) article contains further detail on this.

Remember it’s not possible to edit the underlying HTML of invoice in FreeAgent. The markup in `index.html` is purely for reference. When you go to use your custom theme, the only code you’ll be able to paste into FreeAgent will be CSS.  

## Files and directories
`index.html`  
An example file showing a preview of what your invoice theme will look like. Don’t bother editing any of the HTML, as you can’t edit the HTML for invoices in FreeAgent. Only the CSS can be edited, so the only change you’ll want to make in this file is to amend the stylesheet `href`s.

`base.css`  
Do not edit. These are base styles used to simulate those from the FreeAgent desktop environment.

`gallery`, `images`, and `themes`  
Do not edit. These directories contain imagery referenced by our own invoice themes.

`styles`  
Contains copies of our invoice theme stylesheets. You can use these as the basis for your own theme, but we’d recommend creating duplicates of the files you want, then renaming them. This way you’ll always have the original theme files to compare against your own, in case you need to fix something that’s gone wrong with your custom theme.  
