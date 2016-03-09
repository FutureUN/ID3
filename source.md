<section id="themes">
	<h2>Themes</h2>
		<p>
			Set your presentation theme: <br>
			<!-- Hacks to swap themes after the page has loaded. Not flexible and only intended for the reveal.js demo deck. -->
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/black.css'); return false;">Black (default)</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/white.css'); return false;">White</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/league.css'); return false;">League</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/sky.css'); return false;">Sky</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/beige.css'); return false;">Beige</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/simple.css'); return false;">Simple</a> <br>
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/serif.css'); return false;">Serif</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/night.css'); return false;">Night</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/moon.css'); return false;">Moon</a> -
			<a href="#" onclick="document.getElementById('theme').setAttribute('href','css/theme/solarized.css'); return false;">Solarized</a>
		</p>
</section>

H:
# ID3 Algorithm
(Iterative Dichotomiser 3)

By  [Sebastian Chaves](https://github.com/adamantwharf) - [Daniel Castañeda]() - [Jimmy Pulido](https://github.com/jiapulidoar) - [Miller Cubillos]() 

H:
<!-- .slide: data-background="#ffffff" --> 
# PRESENTATION URL

H:

# Index
<!-- .slide: data-background="#7E2121" --> 
 1. Basic Theorems of Probability<!-- .element: class="fragment" data-fragment-index="0"-->
 1. Bayes' Theorem. <!-- .element: class="fragment" data-fragment-index="1"-->
 1. Entropy <!-- .element: class="fragment" data-fragment-index="2"-->
 1. Decision Tree.  <!-- .element: class="fragment" data-fragment-index="3"-->
 1. ID3 Algorithm. <!-- .element: class="fragment" data-fragment-index="4"-->
	

H:
<!-- .slide: data-background="#005050" -->
#Basic Theorems

V:

###Theorems:

* P(Ω) = 1 
* P(ø) = 0 
* If AЄΩ & Ac is the complement of A:
		P(Ac)= 1-P(A)
* If A, B Є Ω it may happen that: 
      A & B & are exclusive; in this case: 
            P(AUB)=P(A)+P(B) 
      A & B Є Ω & are NOT exclusive: 
            P(A∪B)=P(A)+P(B)-P(A∩B) 

V:

* If A, B & C Є Ω & are independients also:  
      P(A∩B∩C)=P(A)*P(B)*P(C)  
* If A, B & C Є Ω & are dependient events: 
      P(A∩B∩C)=P(A)*P(B⁄A)*P(C⁄(A∩B)) 
* If A, B Є Ω & are coditioned events:

  The probability of A given that B happened is: 
      P(A⁄B)=(P(A∩B))/(P(B)) ; 
      
  The probability of B given that A happened is: 
       P(B⁄A)=(P(A∩B))/(P(A)); 


H:
# Bayes' Theorem
<!-- .slide: data-background="#005050" -->

V:
##Statement of Theorem 
Bayes' theorem is stated mathematically as the following equation:

<img src="images/bayes.png" alt="bayes" with="150" height="150"></img>
>where A and B are events.




H:
# Decision Tree 
<!-- .slide: data-background="#7E2121"  -->
V:
##Structure
* __Nodes__: Names or identifiers of the attributes
* __Branches__: Possible values associated to the node attribute.
* __Leaves__: Sets of examples already classified and labeled with the name of a class.

V:
##Data

* __Attributes__: Are the factors that influence the classification or decision.
* __Class__: Possible values of solution.
* __Examples__: Are the set of combinations of given attributes.

V:
You can choose between 2 business projects: a candy shop or a lemonade stand.

<img src="images/tree1.png" ></img>

Which will you choose? 
Surely the candy shop.

V:
Given the percents of failure and success of each project:

<img src="images/tree2.png" ></img>

Now, which will you choose?

V:
Calculating the expeted values, it's easy make a good choice

<img src="images/tree3.png" ></img>

H:
#Entropy and Gain

V:

##Entropy
A measure of the uncertainty that exists in a system. That is, in a given situation, the probability of occurring each of the possible outcomes.

<img src="images/rare2.jpg" alt="entropy" ></img>

V:
##Interpretation

An example of the binary entropy could get a ball of white or black from a bag.

• If the bag there are 3 white balls and 3 black the result is completely unknown, that is to say uncertainty is high, ie entropy is 1.

<img src="images/bolsa1.png" alt="bayes" with="250" height="250"></img>

V:

• If the bag is 6 black balls the result is known in advance, then there is no uncertainty, and entropy is 0.
 <img src="images/bolsa0.png" alt="bayes" with="250" height="250"></img>
V:
##Gain
>is the difference between the entropy of a node and one of its descendants.

<img src="images/rare1.jpg" alt="Gain" ></img>
 V: 
##Example 
ID3 examines all the attributes and choose the maximum gain, forms the
branch and uses the same process recursively to form sub-trees from the n generated nodes. 

<img src="images/DiagramTree.JPG" alt="Dragram Tree" height="400" ></img>

V:

<img src="images/Tabla1.JPG" alt="Table 1" width="600"></img>
<img src="images/rare3.jpg" alt="" ></img>
V:
<img src="images/Tabla2.JPG" ></img>

H: 
<!-- .slide: data-background="#005050" -->
##Iterative Dichomiser 3 (ID3) Algorithm


