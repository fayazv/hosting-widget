hosting-widget
=============

Widget for selling GoDaddy reseller cPanel

If you have your own storefront pages for the GoDaddy reseller product, this form allows you to add cPanel products to the shopping cart.

Simply change the `prog_id` in the form and you are ready to rock!

## Example

To see a live example, visit http://resellers.github.io/hosting-widget/

## Getting Started

1. Embed the example from `index.html` into your page
2. Remove any plans you do not wish to offer
3. Change your `prog_id` (found on https://www.resellercontrolcenter.com/Settings/default.aspx)
```html
<input type="hidden" name="prog_id" value="domainspricedright"> <!-- enter your prog_id -->
```
###### Sample HTML
Change the **enter_your_prog_id** in the **2** places below (new):
```html
<form method="post" 
    action="https://www.secureserver.net/gdshop/xt_orderform_addmany.asp?prog_id=enter_your_prog_id">
  <input type="hidden" name="tcount" value="1">
  <input type="hidden" name="qty_1" value="1">
  <input type="hidden" name="item_1" value="1">
  <input type="hidden" name="prog_id" value="enter_your_prog_id"> 
  <select name="pf_id_1">
    <option value="32756"> Starter Managed WordPress - US - 1 Month (recurring)</option>
  </select>
  <input type="submit" value="Add to Cart">
</form>

```
