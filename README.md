# js_bottom_tabs

An implementation of Material Design Bottom Navigation using [Materialize](http://materializecss.com/)

## How it works?

It's just the Tabs from Materialize with a nice ripple effect.<br>

Here's an example: <http://codepen.io/kernelmaster/pen/GqjqQw><br>
You can use it with indicators too: <http://codepen.io/kernelmaster/pen/YWGQVa>

## Getting started

1. Include Materialize and jQuery!
2. Include `js_bottom_tabs.css` and `js_bottom_tabs.js` in your project
3. Add the class `bottom_tabs` to the element with the class `tabs`
4. Add the attribute `data-ripple-color` to every `li`-element with the class `tab`. You can use css built-in values like `red`, `grey` etc. but also hex codes like `#212121`
5. If you want to set an active tab, just add the `active` class as usual. If set, this will be the color used as default.
6. This will be the result:

  ```
  <div class="row">
   <div class="col s12">
     <ul class="bottom_tabs tabs">
       <li class="tab col s3"><a class="active" href="#tab1" data-ripple-color="green">Tab 1</a></li>
       <li class="tab col s3"><a href="#tab2" data-ripple-color="red">Tab 2</a></li>
       <li class="tab col s3"><a href="#tab3" data-ripple-color="#212121">Tab 3</a></li>
     </ul>
   </div>
   <div id="tab1" class="col s12">Tab 1</div>
   <div id="tab2" class="col s12">Tab 2</div>
   <div id="tab3" class="col s12">Tab 3</div>
  </div>
  ```

## More

You can hide the tab indicator by adding the class `noindicator` to either your `ul.bottom_tabs` or to the corresponding `li.tab` if you want to hide the indicator only in one tab.
