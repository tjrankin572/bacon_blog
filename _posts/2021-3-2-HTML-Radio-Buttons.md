---
layout: post
title:  "HTML: Basic Inputs Part 1"
date:   2021-03-14 12:00:00 -0700
categories: Coding
author: Tyler Rankin
---


 What is up World?

 I guess that I'm full speed ahead on this whole blog thing.
 One of the things I would love to write about on a consistent basis would be coding tutorials! I've been very lucky to have taught myself enough code in order to land a career in the tech industry. So it'd be nice to share what I've learned along the way.

 Therefore, why not cover the absolute basics that I'm positive any developer whose visiting this blog has probably seen before!

 Today we're going to discuss how to use radio buttons!



 ![Software Developers Have a Disgusted Reaction](https://media.giphy.com/media/W0SLa0YuzWBZ6/giphy.gif)
 \


 
Fine if you're so stuck-up about it, how about we cover three inputs?
Oh, and how about we wrap all these inputs together into a survey project?
Would that quench your thrist?

<iframe src="https://giphy.com/embed/l0EwZ92cG9x9VPC7u" width="480" height="476" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/nba-l0EwZ92cG9x9VPC7u">via GIPHY</a></p>

Sweet, now that we got that out of the way let's get rolling!

Here are the inputs we are going to cover:
<ul>
  <li>Radio Inputs</li>
  <li>Checkboxes</li>
  <li>Dropdown</li>
</ul>

***

<h2>The Form Tag</h2>

<p>Whenever, you're working with inputs, it's a good idea to wrap all of your inputs inside of a form tag. That way our user can start submitting data when they're done with our forms. Since I'm planning to make this a multi-part project series, feel free to fork this codepen below!</p>

<p class="codepen" data-height="364" data-theme-id="dark" data-default-tab="css,result" data-user="tjrankin572" data-slug-hash="rNWPEOE" style="height: 364px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="RankinBacon.blog-SurveyTemplate">
  <span>See the Pen <a href="https://codepen.io/tjrankin572/pen/rNWPEOE">
  RankinBacon.blog-SurveyTemplate</a> by tjrankin572 (<a href="https://codepen.io/tjrankin572">@tjrankin572</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

<p>Without further ado, let's get started.</p>

***

<h2>Making Radio Button</h2>


<p class="codepen" data-height="400" data-theme-id="dark" data-default-tab="html,result" data-user="tjrankin572" data-slug-hash="oNYaJMg" style="height: 600px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="RankinBacon.blog-RadioInput">
  <span>See the Pen <a href="https://codepen.io/tjrankin572/pen/oNYaJMg">
  RankinBacon.blog-RadioInput</a> by tjrankin572 (<a href="https://codepen.io/tjrankin572">@tjrankin572</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

Let's break down these attributes step by step.

<h3>Step 1</h3>
<p>First we'll add in our input tag with a <strong>type</strong> attribute that equals <strong>radio</strong></p>

    <input type="radio">
    <input type="radio">



<h3>Step 2</h3>
<p>Second we'll put in the id of the tag and the value it will produce</strong></p>

    <input type="radio" id="yes" value="YES">
    <input type="radio" id="no" value="NO">


<h3>Step 3</h3>
<p>Now let's add the name attribute so we can associate these buttons to one another.<br>
That way if the user selects one button, it will deselect the other.<br>Every input needs
this anyway, so don't mess it up. </p>

    <input type="radio" id="yes" value="YES" name="BaconFan">
    <input type="radio" id="no" value="NO" name="BaconFan">


 
<h3>Step 4</h3>
<p>Now let's add in some labels for user to understand what the radio buttons represent.<br>
The <strong>for</strong> attribute helps the label to associate itself to the radio button.<br>
That way if the user clicks on the label, it will also select that radio button.</p>

    <input type="radio" id="yes" value="YES" name="BaconFan">
    <label for="yes">Yes</label>

    <input type="radio" id="no" value="NO" name="BaconFan">
    <label for="no">No</label>  


***


<h2>Making Checkboxes</h2>


<p class="codepen" data-height="400" data-theme-id="dark" data-default-tab="html,result" data-user="tjrankin572" data-slug-hash="bGBzKRW" style="height: 600px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="RankinBacon.blog-Checkboxes">
  <span>See the Pen <a href="https://codepen.io/tjrankin572/pen/bGBzKRW">
  RankinBacon.blog-Checkboxes</a> by tjrankin572 (<a href="https://codepen.io/tjrankin572">@tjrankin572</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

<h3>Step One</h3>

<p>Set the type of the input to checkbox and the approriate id</p>

    <input type="checkbox" id="pepperoni-btn">


<h3>Step Two</h3>

<p>Now add the name and value attributes for the checkboxes.</p>

    <input type="checkbox" id="pepperoni-btn" name="toppings" value="PEPPERONI">

<h3>Step Three</h3>

<p>Great now let's add in our label so the user undestands what this checkbox does.<br>Make sure to the <strong>for</strong> attribute is associated with your checkbox id.</p>

    <input type="checkbox" id="pepperoni-btn" name="toppings" value="PEPPERONI">
    <label for="pepperoni-btn">Pepperoni</label>


<h3>Step Four</h3>

<p>Now just add in the rest of your checkboxes and you're good to go! Make sure they all still have the same name tag</p>


    <input type="checkbox" id="pepperoni-btn" name="toppings" value="PEPPERONI">
    <label for="pepperoni-btn">Pepperoni</label>

    <input type="checkbox" id="extra-cheese-btn" name="toppings" value="EXTRA_CHEESE">
    <label for="extra-cheese-btn">Extra Cheese</label>

    <input type="checkbox" id="mushroom-btn" name="toppings" value="MUSHROOM">
    <label for="mushroom-btn">Mushroom</label>

    <input type="checkbox" id="pineapple-btn" name="toppings" value="PINEAPPLE">
    <label for="pineapple-btn">Pineapple</label>

    <input type="checkbox" id="bacon-btn" name="toppings" value="BACON">
    <label for="bacon-btn">Bacon</label>

***

<h2>Making Dropdowns</h2>


<p class="codepen" data-height="400" data-theme-id="dark" data-default-tab="html,result" data-user="tjrankin572" data-slug-hash="eYBxKKQ" style="height: 600px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="RankinBacon.blog-Dropdowns">
  <span>See the Pen <a href="https://codepen.io/tjrankin572/pen/eYBxKKQ">
  RankinBacon.blog-Dropdowns</a> by tjrankin572 (<a href="https://codepen.io/tjrankin572">@tjrankin572</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://cpwebassets.codepen.io/assets/embed/ei.js"></script>

<h3>Step One</h3>

<p>In order to setup a dropdown, let's first add in our select tag. We'll also add in our label tag, get our id and name attributes all setup as well.</p>

    <label for="hogwarts-house">Select a House</label>

    <select id="hogwarts-house" name="hogwarts-house">
    </select>


<h3>Step Two</h3>

<p>Right now, our dropdown is empty! Let's fix that by adding in some options inside our select tag. Make sure to add in the value for each of our options.</p>

    <label for="hogwarts-house">Select a House</label>

    <select id="hogwarts-house" name="hogwarts-house">
      <option value="gryffindor">Gryffindor</option> 
      <option value="slytherin">Slytherin</option> 
      <option value="ravenclaw">Ravenclaw</option> 
      <option value="hufflepuff">Hufflepuff</option> 
    </select>


<h3>Step Three</h3>

<p>Great! Now we can select our house! But there's only one problem. It selects Gryffindor by default! While that is my house, I don't want the user to accidently pick that if they're in Ravenclaw.<br> So let's add in a placeholder option that will show up initially but can't be selected once the user interacts with the dropdown.<br> For our new option tag, add the <strong>selected</strong> attribute that will make it our default option. Then add <strong>disabled</strong> and <strong>hidden</strong> to prevent the user from accidently selecting the placeholder option. <br> Feel free to play around with this by removing this attributes and interacting with the dropdown to see what happens!</p>

    <label for="hogwarts-house">Select a House</label>

    <select id="hogwarts-house" name="hogwarts-house">

      <option value="none" selected disabled hidden>Select an option</option>

      <option value="gryffindor">Gryffindor</option> 
      <option value="slytherin">Slytherin</option> 
      <option value="ravenclaw">Ravenclaw</option> 
      <option value="hufflepuff">Hufflepuff</option> 
    </select>

***

<h2>Conclusion</h2>
<p>That is it! Congratulations on making this far! Thanks for joining me on the first part of this multi-part survey form project. Once the next part is up I'll update this post in order to link you directly to that post.</p>
