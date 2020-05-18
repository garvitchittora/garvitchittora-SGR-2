# COVID-19 (ALL LIVE UPDATES) DOCUMENTATION :


## DESCRIBTION :
This Project contains all essential information about 2019–20 coronavirus pandemic link symptoms , advisory given by government and one can see statistics of number of covid cases and death around the world . This project also contain a survey form asking about where you were in these 14 days and its dates . Through this project one can donate money to INDIAN GOVERNMENT .Methods of how to wash hands is also mention on the webpage .It also contain a section where you can find some good article for entertainment .

## LANGUAGES USED IN WEBPAGE:
```
	1) HTML
	2) CSS
	3) JAVASCRIPT ( JQUERY )
 ```
## HOW TO USE THIS WEBPAGE :
	
  #### There are two ways:
	
   **1) By link**: 
		Just click on the link given below that will take you directly to the webpage.
	
[Webpage Link](https://garvitchittora.github.io/garvitchittora-SGR-2/)
    	
    
   **2) Git Clone**:
		For this method you should gave git bash installed on your workstation and then follow the given below
    		commands
		
		Step 1) Open Git Bash .
		
		Step 2) Git clone https://github.com/garvitchittora/garvitchittora-SGR-2.git (Wait till 100% is 
		completed)
		
		Step 3) Open garvitchittora-SGR-2 (which has whole code of webpage )
		
		Step 4) Then you will find index.html in garvitchittora-SGR-2 folder .
		Click on it that will take you to the webpage .

## File In This Project :
#### This project has 3 files :
  
**1) index.html** - which is a html file contain html/javascript code of the webpage.

**2) main.css** - which is a css file contain css code of the webpage.

**3) images folder** - which contains all images used in webpage .

## DIFFERENT HTML / CSS SECTIONS OF THE WEBPAGE:
#### NO OF SECTIONS : 11

**1) BANNER -** This section has Banner of the webpage which has a image ( which rotate 360 degree in 10
seconds for infinite time ) , Heading , Sub Heading and a  MEET THE DOCTOR Button ( which show Doctor is
available or not ) . This section has 1 function whose function is when this button is hoved it changes 
some of its css propety and text inside the button .  

**2) STAT SECTION -**  This section has all the statistics about COVID - 19 like Total number of coronavirus 
cases around the world , Total number of recovered cases around the world ,Total number of Deaths and Total 
number of countries which are going through Covid -19 . This section also has a map ( showing regions around
the world on the basis of number of cases in the country ) and Stats like total number of cases and total 
number of Deaths in the country of Top 10 Countries which are going through COVID  . It also has a javasript
function which increase value of the section slowly (in 4 second ) to a fixed defined value . It also has a 
background image which is a world map .  

**3) PROFILE -** This section has my picture along with some basic information about me , which display when
someone hover over the developer button in fixed header along with link of my instagram ,
facebook , linkedin , twitter , github account. 

**4) FIXED HEADER -** This section has a header in which is fixed after a particular pixels ( 600 px ) before 
that it is not displayed . It has website logo , a survey form ( which is a general survey asking about 
where you were in these 14 days and Date picker through which you can select initial and final date ) , 
WHO ( world health organisation's webpage link ) , DONATE ( By clicking on it you are redirected to
government of india's webpage where you can donate money ) , DEVELOPER ( which on hover open profile
section ) . This section has 3 javascript functions (1 for date picker , 1 position of fixed header and 1 for
developer section indepth functions are explained below ) .

**5) SAFE-ACTION -** This section consist of correct method of how one should wash hands . It has 12 parts 
each having one image (On hover it rotates 360 degree in 4 seconds for infinite time till the image is hovered) 
shows the different steps of how to wash hands and discribtion about the step . 

**6) MID SECTION -** This section consist of information about symptoms of COVID , advisory given by 
government and one can see statistics of number of covid cases and death around the world . It has 3 section 
each having one image and Heading of that part . If we hover on any of the part , it transform to 1.05 times 
of its size. 

**7) LOWER MID -** This section consist of section where you can find some good article for entertainment.
It has 4 section each having one image of the article and discribtion about the article . If we hover on any
of the part , it lifts up by 0.5 % of the section hight . 

**8) FOOTER -** This section has footer of the webpage and copyright bar along with link of my instagram ,
facebook , linkedin , twitter , github account . It also has informational link of symptoms , advice ,
stats , etc.

**9) Scroll -**  In this section color and orientation of the normal scroll is changed so that it match 
the total theme of the webpage.  

**10) Move to the top -**  This section consist of a button which take the webpage directly to the top through 
two javascript function mentioned below one for its positioning and another function task is when we click
on the move to the top button it takes to the top . It also changes its color on hover and position of this 
section is fixed with z-index.

**11) PRELOADER** - This section consist of a simple loader ( a page which you see untill whole webpage is 
completely loaded for use ) which has 3 div which animate and a text (GO CORONA GO....) . It consist of a 
javasript function that change its css property by adding a class "hidden" which has css property 
visibility:hidden , after whole webpage is loaded . 

## FUNCTIONS OF JAVASCRIPT USED IN THE WEBPAGE:

#### There are 8 javascript functions used on the webpage :
````
Serial Number)
  a) Use

  b) Function Explaination	
````
		1)	
			a) This function is used to add a class in "overlay" when full webpage is loaded .

			b) The addEventListener() method attaches an event handler to an element without overwriting 
			existing event handlers,syntax element.addEventListener(event, function) . I had used 
			load event in addEventListener() which call the function when the webpage is completely loaded . 
			
				//window.addEventListener("load",function(){

			"loader" is a constant which has all elements of class name "overlay" .	

	    			//const loader=document.querySelector(".overlay");
	    	
	    	HTMLElementObject.className += class adds the "class" to the class name of the HTMLElementObject . we
		know loader has element with class name "overlay" . After the below given line is executed class name
		of loader is changed to "overlay hidden" . "hidden" class hides the loader after the webpage is loaded .
	    	
	    			//loader.className+=" hidden";
				//});


       	2)
       		a) This function is used to make operations on datepicker used in survey form and decide what will be 
		the value of the datepicker .
			
			b)A date-picker of jQuery UI is used to provide a calendar to the user to select the date from a
			Calendar. This date picker usually connected to a text-box so user selection of date from the 
			calendar can be transferred to the textbox.
			
			Element is seached with name "datefilter" and of input category . In this autoupdate input is
			placed false means value is not autoupdated .
		        //$(function() {
		            //$('input[name="datefilter"]').daterangepicker({
		            //autoUpdateInput: false,
		            //locale: {
		               //cancelLabel: 'Clear'
		            //}
		        //});

		    	When we click on apply in "datefilter" this function change the value of "datefilter" with
			"startDate - endDate" in MM/DD/YYYY format .   
		        //$('input[name="datefilter"]').on('apply.daterangepicker', function(ev, picker) {
		               //$(this).val("    "+picker.startDate.format('MM/DD/YYYY') + ' - ' + 
			       //picker.endDate.format('MM/DD/YYYY'));
		        //});

		    When we click on cancel in "datefilter" this function change the value of "datefilter" with "       
		    Add Dates Here By Clicking On It" .    	
		        //$('input[name="datefilter"]').on('cancel.daterangepicker', function(ev, picker) {
		               //$(this).val('       Add Dates Here By Clicking On It');
		            //});
		        //});
         

        3) 	
        	a) This function is used to position the fixed header after 600 px and add some class to it .
			
		b) The "onscroll" event occurs when an element's scrollbar is being scrolled. When someone scroll, it
		calls "myFunction" function.
		    	
		    	//window.onscroll = function() {myFunction()};

		    The getElementById() method returns the element that has the ID attribute with the specified value
		    ,whose syntax is document.getElementById(elementID). "header" is a variable which has the element
		    whose id is "myHeader" .
		    	
		    	//var header = document.getElementById("myHeader");

		    "myFunction" is a function which is being called by onscroll event as mentioned above.	

		    	//function myFunction() {
			
		    "pageYOffset" properties returns the pixels the current document has been scrolled from the upper
		    left corner of the window, vertically , whose syntax is window.pageYOffset . If "pageYOffset" is
		    greater then 600 the it will move inside the "if  loop" .	
			    	//if (window.pageYOffset > 600) {

			The classList property returns the class name(s) of an element, as a DOMTokenList object.This
			property is useful to add, remove and toggle CSS classes on an element. It will add "sticky"
			class to the class list of header .   	
			           //header.classList.add("sticky");

			The css() method sets or returns one or more style properties for the selected elements.
			Element with id "myHeader" is selected and in css of it sets "display" with "block" .           
			           //$("#myHeader").css("display","block");

			If "pageYOffset" is not greater then 600 the it will move inside the "else  loop" .           
			        //}else {

			It will remove "sticky" class to the class list of header .        
			           //header.classList.remove("sticky");

			Element with id "myHeader" is selected and in css of it sets "display" with "none" .           
			           //$("#myHeader").css("display","none");
			       	//}
			    //}
        
        4) 	
        	a) This function is used to position MOVE TO TOP section and decide when it will fadeIn or FadeOut .
			
		b) The "onscroll" event occurs when an element's scrollbar is being scrolled. When someone scroll it 
		calls  function.
	        	//$(window).scroll(function() {

	        The scrollTop property sets or returns the number of pixels an element's content is scrolled vertically.
		If it is greater then 600 then it will move inside the "if"  loop.	
		            //if ($(this).scrollTop() > 600 ) {

		    The jQuery stop() method is used to stop an animation or effect before it is finished.The stop()
		    method works for all jQuery effect functions, including sliding, fading and custom animations ,
		    whose syntax is "$(selector).stop(stopAll,goToEnd);" . This "$('.scrolltop:hidden')" will return
		    the element with class "scrolltop" when it is "hidden" . The fadeIn() method gradually changes 
		    the opacity, for selected elements, from hidden to visible (fading effect).       
		            	//$('.scrolltop:hidden').stop(true, true).fadeIn();

		    If it is not greater then 600 then it will move inside the "else"  loop.        
		            //} else {

		    The fadeOut() method gradually changes the opacity, for selected elements, from visible to 
		    hidden (fading effect).        
		            //$('.scrolltop').stop(true, true).fadeOut();
		            //}
		        //});

	    
	    5)	
	    	a) This function is used when we click on MOVE TO TOP button it takes the webpage to 0 px  .
			
		b) The click() method simulates a mouse-click on an element.This method can be used to execute a click on
		an element as if the user manually clicked on it , syntax HTMLElementObject.click() . It calls the
		function on click .	
		        //$(".scrolltop").click(function() {

		    The animate() method performs a custom animation of a set of CSS properties.This method changes an 
		    element from one state to another with CSS styles. The CSS property value is changed gradually, to 
		    create an animated effect, syntax (selector).animate({styles},speed,easing,callback) . It select
		    html's body on animate it to scroll top to 0 px in 1000 milliseconds.    
		            //$("html, body").animate({ scrollTop: 0 }, "1000");
		            //return false;
		        //});

        6)	
        	a) This function is used to animate the numbers present in the STAT section .
			
		b) The each() method specifies a function to run for each matched element. If there are number of 
		element with class name ".count-number" it will call function for each element .
	            //$('.count-number').each(function () {

	        The prop() method sets or returns properties and values of the selected elements.When this method is used
		to return the property value, it returns the value of the FIRST matched element , syntax 
		$(selector).prop(property,value) .It will initialise property "Counter" of element to "0" and animate it
		to "$(this).text()" in 4000 milliseconds .    
	               //$(this).prop('Counter',0).animate({
	               		//Counter: $(this).text()
	           		//}, {
		               //duration: 4000,

		    "easing" specifies the speed of the element in different points of the animation.            
		               //easing: 'swing',
		               //step: function (now) {

		    The ceil() method rounds a number UPWARDS to the nearest integer, and returns the result means we will
		    not get a decimal value , we will only get integer values .           
		                   //$(this).text(Math.ceil(now));
	               		//}
	           		//});
	         	//});


        7)
         	a) This function is used when a user hover over the element with id "developer" it changes css of element
		whose id is "profile" and according to width of the document also it changes the css .
			
		b) The hover() method specifies two functions to run when the mouse pointer hovers over the selected
		elements , syntax $(selector).hover(inFunction,outFunction) . When cursor is hovered over element with
		id "developer" function is called . 
		        //$("#developer").hover(function(){

		    The css() method sets or returns one or more style properties for the selected elements.Element with
		    id "profile" is selected and in css of it sets "display" with "block" .    
		            //$("#profile").css("display", "block");

		    "width" is a variable through which we get the width of document .         
		            //var width = $(document).width();

		    If , "width" is less than or equal to 768 . Element with id "profile" is selected and in css
		    of it sets "width" , "margin-left" with "40%" and "50%" respectively.         
		            //if(width<=768){
		               //$("#profile").css("width","40%");
		               //$("#profile").css("margin-left","50%")
		            //}  

		    Else , Element with id "profile" is selected and in css of it sets "width" , "margin-left" with "20%"
		    and "75%" respectively.         
		            //else{
		               //$("#profile").css("width","20%");
		               //$("#profile").css("margin-left","75%")
		            //} 

		    If , Element is not hover then below given function is called and css property "display" of element
		    with id "profile" is changed to "none" .       
		           //}, function(){
		           //$("#profile").css("display", "none");
		        //});


        8)
         	a) This function is used when a user hover over the element with class "meet_doctor" it changes css of that
		element with its text .
			
		b) The hover() method specifies two functions to run when the mouse pointer hovers over the selected elements
		, syntax $(selector).hover(inFunction,outFunction) . When cursor is hovered over element with class
		"meet_doctor" function is called , that changes some of its css properties and its text with backgound
		color of its parent div .  	
		        //$(".meet_doctor").hover(function(){
		            //$(this).text("AVAILABLE!");
		            //$(this).css("margin-left","22%");
		            //$(this).css("font-size","17px");
		            //$("#meet-doctor-div").css("background-color","green");

		    If , Element is not hover then below given function is called , that changes some of its css 
		    properties and its text with backgound color of its parent div .
		         //}, function(){
		            //$(this).text("MEET THE DOCTOR");
		            //$(this).css("font-size","17px");
		            //$(this).css("margin-left","12%");
		            //$("#meet-doctor-div").css("background-color","");
		        //});
         


## ScreenShots Of The Webpage :


1) 
![](images/screenshot/Screenshot%20(198).png)


2) 
![](images/screenshot/Screenshot%20(199).png)


3)
![](images/screenshot/Screenshot%20(201).png)


4)
![](images/screenshot/Screenshot%20(203).png)


5)
![](images/screenshot/Screenshot%20(204).png)


6)
![](images/screenshot/Screenshot%20(205).png)


## Author :
Garvit Chitttora , I am a First year student at IIIT Allahabad . I had made this webpage for selection in a competition organised by WebD wing of GeekHeaven ,IIIT A .

Contact On : iit2019142@iiita.ac.in for more information .
