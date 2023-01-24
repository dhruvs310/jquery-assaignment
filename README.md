# jquery-assaignment
MODULE: 5 (JQuery Basic, Effects & Advance)
	      Name: Dhruv Shrimali

1. What is JQuery?
Ans. jQuery is a small, light-weight and fast JavaScript library. It is cross-platform and
supports different types of browsers. It is also referred as ?write less do more? because
it takes a lot of common tasks that requires many lines of JavaScript code to
accomplish, and binds them into methods that can be called with a single line of code
whenever needed. It is also very useful to simplify a lot of the complicated things from JavaScript, like AJAX calls and DOM manipulation.
o jQuery is a small, fast and lightweight JavaScript library.
o jQuery is platform-independent.
o jQuery means "write less do more".
o jQuery simplifies AJAX call and DOM manipulation.

2.How to Apply CSS Using JQuery, How to Add Class and Remove Class in JQuery, JQuery Animation?
Ans. You can add css by jQuery in two ways
1. Add css to your element
$('css_selecttor').css('css_property' : 'property_value', 'css_property' :
'property_value');
2. By adding class defined in css means you can add class written in css file by
jquery
$('your_element').addClass('css_class_name');

ADD class and remove class in jquery:
Add class in Jquery
Jquery has method calle addClassd () which can be used to
add one or more class to the DOM elements.
It takes class names in the string format.
 
//Add red class to the
//element with id abc
$("#abc").addClass('red');

Copy
To add multiple classes pass them space separated
in string format.

//Add multiple class to the
//element with id abc
$("#abc").addClass('red yellow pink blue');

Copy
addClass() method assigns the given list of classes to all
the selected element.
 
//Add multiple class to the
//element with input type text
$("input[type='text']").addClass('red yellow pink blue');

Copy
If the class is already present then it will overwrite it.
Remove class using Jquery
Jquery has method called removeClass() which can be
used to remove one or more class from the DOM elements.

//Remove red class from the
//element with id abc
$("#abc").removeClass('red’)

JQUERY ANIMATION
"Animate" an element, by changing its height:
$("button").click(function(){
$("#box").animate({height: "300px"}); })

Definition and Usage
The animate() method performs a custom animation of a set of CSS
properties.
This method changes an element from one state to another with CSS styles.
The CSS property value is changed gradually, to create an animated effect.
Only numeric values can be animated (like "margin:30px"). String values
cannot be animated (like "background-color:red"), except for the strings
"show", "hide" and "toggle". These values allow hiding and showing the
animated element.

3. How to create slider with animation
Ans.
 <div id="slider"> 
            <div class="dp-wrap"> 
              <div id="dp-slider">
          
                <div class="dp_item" data-class="1" data-position="1">
                  <div class="dp-content">
                    
                    <h2>Slide 1</h2>
                    <p> This is Slide 1 </p>
                    <a href="#" class="site-btn">Read More…</a>
                  </div>
                  <div class="dp-img">
                    <img class="img-fluid" src="https://images.pexels.com/photos/14254235/pexels-photo-14254235.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load" alt="investing">
                  </div>
                </div>
          
                <div class="dp_item" data-class="2" data-position="2">
                  <div class="dp-content">
                    
                    <h2>Slide 2</h2>
                    <p> This is Slide 2 </p>
                    <a href="#" class="site-btn">Read More…</a>
                  </div>
                  <div class="dp-img">
                    <img class="img-fluid" src="https://images.pexels.com/photos/14254235/pexels-photo-14254235.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load" alt="investing">
                  </div>
                </div>
          
                <div class="dp_item" data-class="3" data-position="3">
                  <div class="dp-content">
                    
                    <h2>Slide 3</h2>
                    <p> This is Slide 3 </p>
                    <a href="#" class="site-btn">Read More…</a>
                  </div>
                  <div class="dp-img">
                    <img class="img-fluid" src="https://images.pexels.com/photos/14254235/pexels-photo-14254235.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load" alt="investing">
                  </div>
                </div>
          
                <div class="dp_item" data-class="4" data-position="4">
                  <div class="dp-content">
                    
                    <h2>Slide 4</h2>
                    <p> This is Slide 4 </p>
                    <a href="#" class="site-btn">Read More…</a>
                  </div>
                  <div class="dp-img">
                    <img class="img-fluid" src="https://images.pexels.com/photos/14254235/pexels-photo-14254235.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load" alt="investing">
                  </div>
                </div>
              </div>
              
              <span id="dp-next">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 51.401 51.401">
                  <defs>
                    <style>
                      .cls-1 {
                        fill: none;
                        stroke: #fa8c8c;
                        stroke-miterlimit: 10;
                        stroke-width: 7px;
                      }
                    </style>
                  </defs>
                  <path id="Rectangle_4_Copy" data-name="Rectangle 4 Copy" class="cls-1" d="M32.246,0V33.178L0,31.953" transform="translate(0.094 25.276) rotate(-45)"/>
                </svg>
              </span>
          
              <span id="dp-prev">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 51.401 51.401">
                  <defs>
                    <style>
                      .cls-1 {
                        fill: none;
                        stroke: #fa8c8c;
                        stroke-miterlimit: 10;
                        stroke-width: 7px;
                      }
                    </style>
                  </defs>
                  <path id="Rectangle_4_Copy" data-name="Rectangle 4 Copy" class="cls-1" d="M32.246,0V33.178L0,31.953" transform="translate(0.094 25.276) rotate(-45)"/>
                </svg>
              </span>
   <ul id="dp-dots">
                <li data-class="1" class="active"></li>
                <li data-class="2"></li>
                <li data-class="3"></li>
                <li data-class="4"></li>
              </ul>
            </div>
          </div>
