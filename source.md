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
 1. Decision Tree.  <!-- .element: class="fragment" data-fragment-index="2"-->
 1. ID3 Algorithm. <!-- .element: class="fragment" data-fragment-index="3"-->
	

H:
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
asfdasdfasdf

H: 
<!-- .slide: data-background="#005050" -->
##Iterative Dichomiser 3 (ID3) Algorithm

