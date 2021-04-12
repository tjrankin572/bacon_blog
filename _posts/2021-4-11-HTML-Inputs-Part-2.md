---
layout: post
title:  "HTML: Basic Inputs Part 2"
date:   2021-04-10 12:00:00 -0700
categories: Coding
author: Tyler Rankin
---

## HTML Inputs: Basic Inputs Part 2
Alright, welcome to part 2 where we're covering the very basics about HTML Inputs, so let's dig in & finish out this project. As the title indicates, this lesson contiues from the previous. However, I decided to restart the Codepen project, so that you don't have to scroll to the bottom to see the examples. If you were working on from a project in the previous post feel free to simply add the code you learn here to that project.

This post is going to be less complicated than the previous post. It relies on the fact that you've worked on the importance of a couple of attributes such as for or name. Therefore, it won't have any step structure like the previous one did.

### Text Inputs

First up on our list is the mightly humble, text input.

Let's take a look at an example.

<p class="codepen" data-height="364" data-theme-id="dark" data-default-tab="html,result" data-user="tjrankin572" data-slug-hash="NWdyvzy" style="height: 364px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="RankinBacon.blog-Text Inputs">
  <span>See the Pen <a href="https://codepen.io/tjrankin572/pen/NWdyvzy">
  RankinBacon.blog-Text Inputs</a> by tjrankin572 (<a href="https://codepen.io/tjrankin572">@tjrankin572</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

Awesome, now let's take a look at the code.

    <label for="fname"> First Name </label>
 
    <input type="text" id="fname" name="fname"></input>
     
    <label for="lname"> Last Name </label>
     
    <input type="text" id="lname" name="lname"></input>

    <label for="movie" > What is your favorite movie? </label>
    
    <input type="text" id="movie" placeholder="i.e. John Wick" name=""></input>

Remember to give each of the labels a <b>for</b> attribute assigned with their respective ids.
That way if the user clicks on the label, the cursor will select the text input.

Furthermore, as you can see for that last input I went ahead and used the <b>placeholder</b> attribute
in order to put in some example text inside of our text inputs.

## TextAreas

Not so bad so far eh?

Now let's try gathering more qualitative information using a textbox that lets the user put in multiple lines of text if they wish.

<p class="codepen" data-height="364" data-theme-id="dark" data-default-tab="html,result" data-user="tjrankin572" data-slug-hash="RwKQxzV" style="height: 364; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="RankinBacon.blog-TextArea">
  <span>See the Pen <a href="https://codepen.io/tjrankin572/pen/RwKQxzV">
  RankinBacon.blog-TextArea</a> by tjrankin572 (<a href="https://codepen.io/tjrankin572">@tjrankin572</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

Okay...I might have allowed a cringy experience I had a convention yesterday to influence the title of that question. Let's move on to the code.


    <label>Describe an experience that triggered every worst nerd cringe in your body?</label>

    <textarea type="textareas" rows=5 cols=58></textarea>


As you can see instead of using the input tag we're using <b>textarea</b>. One to adjust the size of the textarea is with the <b>rows</b> and <b>cols</b> attributes. 

I gave you a lot of room just in case you experienced a lot that you needed to....vent about......anything....

Oh! Also remember that those rows and cols attributes are <b>not respoinsive</b>. So shrinking or growing the screen won't affect the size of the textbox. You should use css for the requirement instead.

## Numbers

We can have text inputs that only accept numbers!

<p class="codepen" data-height="364" data-theme-id="dark" data-default-tab="html,result" data-user="tjrankin572" data-slug-hash="qBRxxbN" style="height: 364px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="RankinBacon.blog-Numbers">
  <span>See the Pen <a href="https://codepen.io/tjrankin572/pen/qBRxxbN">
  RankinBacon.blog-Numbers</a> by tjrankin572 (<a href="https://codepen.io/tjrankin572">@tjrankin572</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

*ahem* Okay, so you see what it does by playing with the input.
The user can add in numbers as valid inputs.

    <label for='age'>How old are you?</label>
     
    <input type='number' min=0 max=120 id='age' name='age'></input>
 
    <label for='pizza'>How many pizzas can you eat in one session?</label>
    
    <input type='number' step=5 id='pizza' name='pizza'> </input>


The <b>min</b> and <b>max</b> attributes help us set a range for the values we want. So the only acceptable numbers will be between 0 and 120.

The <b>step</b> attribute, increments the number by the amount that we specify. So it will increment up or down by 5 in the example above.

<h2>Conclusion</h2>

See not that bad.

While I covered the HTML inputs that are the most used, there are still plenty of inputs to familiarize yourself with. I did have more content planned for this post but in the end I decided to push that off for a CSS programming tutorial project that I'm going to start writing about. Therefore, I'm gonna leave a link to an MDN article breaking down more inputs that you can play around with. 

Quickly, scrolling through that MDN just how many inputs I could cover including the email and color picker. However, I'm assuming that most people reading along know about HTML or can just read along. Either way, I want to start teaching meatier material such as CSS. Until then, I will see you in the next tutorial!


<h2>Resources</h2>


<a href="https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types">HTML5 Input Types</a>






