# jquery-addarrow-plugin
short plugin for adding an arrow at the end of any element html.




-------------------------

example.html
<ul>
  <li>Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</li>
  <li class="addArrow">Aliquam tincidunt mauris eu risus.</li>
  <li>Vestibulum auctor dapibus neque.</li>
</ul>


---------------
plugin.js


(function($) {
$.fn.addArrow = function() {
  return this.each(function() {
    var el = $(this);
    el.html(el.html() + " &rarr;"); 
  });
};
})(jQuery)

jQuery(".addArrow")
  .addArrow();
  
  
  
  
  
  
  
  output::::
Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
Aliquam tincidunt mauris eu risus. →
Vestibulum auctor dapibus neque.
