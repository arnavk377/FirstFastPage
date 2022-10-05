---
keywords: fastai
description: Learning about lists and dictionaries.
title: Python Week 2
toc: true 
badges: true
comments: true
categories: [jupyter, week2, python, csp]
image: 
nb_path: _notebooks/2022-08-29-Python-Dictionaries.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-29-Python-Dictionaries.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Running-the-Code">Running the Code<a class="anchor-link" href="#Running-the-Code"> </a></h2><p>I ran the given code from the APCSP website. I hypothesize that strings, floats, and integers are primitive, as they are simpler, and usually one value. This means that dictionaries and lists are collections, as they are a collection of multiple values.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What is the variable name/key?&quot;</span><span class="p">,</span> <span class="s2">&quot;value?&quot;</span><span class="p">,</span> <span class="s2">&quot;type?&quot;</span><span class="p">,</span> <span class="s2">&quot;primitive or collection, why?&quot;</span><span class="p">)</span>
<span class="n">name</span> <span class="o">=</span> <span class="s2">&quot;John Doe&quot;</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">name</span><span class="p">))</span>

<span class="nb">print</span><span class="p">()</span>


<span class="c1"># variable of type integer</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What is the variable name/key?&quot;</span><span class="p">,</span> <span class="s2">&quot;value?&quot;</span><span class="p">,</span> <span class="s2">&quot;type?&quot;</span><span class="p">,</span> <span class="s2">&quot;primitive or collection, why?&quot;</span><span class="p">)</span>
<span class="n">age</span> <span class="o">=</span> <span class="mi">18</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;age&quot;</span><span class="p">,</span> <span class="n">age</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">age</span><span class="p">))</span>

<span class="nb">print</span><span class="p">()</span>

<span class="c1"># variable of type float</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What is the variable name/key?&quot;</span><span class="p">,</span> <span class="s2">&quot;value?&quot;</span><span class="p">,</span> <span class="s2">&quot;type?&quot;</span><span class="p">,</span> <span class="s2">&quot;primitive or collection, why?&quot;</span><span class="p">)</span>
<span class="n">score</span> <span class="o">=</span> <span class="mf">90.0</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;score&quot;</span><span class="p">,</span> <span class="n">score</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">score</span><span class="p">))</span>

<span class="nb">print</span><span class="p">()</span>

<span class="c1"># variable of type list (many values in one variable)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What is variable name/key?&quot;</span><span class="p">,</span> <span class="s2">&quot;value?&quot;</span><span class="p">,</span> <span class="s2">&quot;type?&quot;</span><span class="p">,</span> <span class="s2">&quot;primitive or collection?&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What is different about the list output?&quot;</span><span class="p">)</span>
<span class="n">langs</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Python&quot;</span><span class="p">,</span> <span class="s2">&quot;JavaScript&quot;</span><span class="p">,</span> <span class="s2">&quot;Java&quot;</span><span class="p">]</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;langs&quot;</span><span class="p">,</span> <span class="n">langs</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">langs</span><span class="p">),</span> <span class="s2">&quot;length&quot;</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">langs</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;- langs[0]&quot;</span><span class="p">,</span> <span class="n">langs</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="nb">type</span><span class="p">(</span><span class="n">langs</span><span class="p">[</span><span class="mi">0</span><span class="p">]))</span>

<span class="nb">print</span><span class="p">()</span>

<span class="c1"># variable of type dictionary (a group of keys and values)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What is the variable name/key?&quot;</span><span class="p">,</span> <span class="s2">&quot;value?&quot;</span><span class="p">,</span> <span class="s2">&quot;type?&quot;</span><span class="p">,</span> <span class="s2">&quot;primitive or collection, why?&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;What is different about the dictionary output?&quot;</span><span class="p">)</span>
<span class="n">person</span> <span class="o">=</span> <span class="p">{</span>
    <span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span>
    <span class="s2">&quot;age&quot;</span><span class="p">:</span> <span class="n">age</span><span class="p">,</span>
    <span class="s2">&quot;score&quot;</span><span class="p">:</span> <span class="n">score</span><span class="p">,</span>
    <span class="s2">&quot;langs&quot;</span><span class="p">:</span> <span class="n">langs</span>
<span class="p">}</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;person&quot;</span><span class="p">,</span> <span class="n">person</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">person</span><span class="p">),</span> <span class="s2">&quot;length&quot;</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">person</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;- person[&quot;name&quot;]&#39;</span><span class="p">,</span> <span class="n">person</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">],</span> <span class="nb">type</span><span class="p">(</span><span class="n">person</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">]))</span>

<span class="nb">print</span><span class="p">(</span><span class="n">langs</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="c1"># Will output &quot;Java&quot;</span>
<span class="nb">print</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>What is the variable name/key? value? type? primitive or collection, why?
name John Doe &lt;class &#39;str&#39;&gt;

What is the variable name/key? value? type? primitive or collection, why?
age 18 &lt;class &#39;int&#39;&gt;

What is the variable name/key? value? type? primitive or collection, why?
score 90.0 &lt;class &#39;float&#39;&gt;

What is variable name/key? value? type? primitive or collection?
What is different about the list output?
langs [&#39;Python&#39;, &#39;JavaScript&#39;, &#39;Java&#39;] &lt;class &#39;list&#39;&gt; length 3
- langs[0] Python &lt;class &#39;str&#39;&gt;

What is the variable name/key? value? type? primitive or collection, why?
What is different about the dictionary output?
person {&#39;name&#39;: &#39;John Doe&#39;, &#39;age&#39;: 18, &#39;score&#39;: 90.0, &#39;langs&#39;: [&#39;Python&#39;, &#39;JavaScript&#39;, &#39;Java&#39;]} &lt;class &#39;dict&#39;&gt; length 4
- person[&#34;name&#34;] John Doe &lt;class &#39;str&#39;&gt;
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Using-Append">Using Append<a class="anchor-link" href="#Using-Append"> </a></h2><p>Using the <code>.append()</code> function to add more information. Using InfoDb from the APCSP repository. Additionally, this demonstrates using user input to add information to InfoDb.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">InfoDb</span> <span class="o">=</span> <span class="p">[]</span>

<span class="c1"># InfoDB is a data structure with expected Keys and Values</span>

<span class="c1"># Append to List a Dictionary of key/values related to a person and cars</span>
<span class="n">InfoDb</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;FirstName&quot;</span><span class="p">:</span> <span class="s2">&quot;John&quot;</span><span class="p">,</span>
    <span class="s2">&quot;LastName&quot;</span><span class="p">:</span> <span class="s2">&quot;Mortensen&quot;</span><span class="p">,</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="s2">&quot;October 21&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Residence&quot;</span><span class="p">:</span> <span class="s2">&quot;San Diego&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="s2">&quot;jmortensen@powayusd.com&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Owns_Cars&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;2015-Fusion&quot;</span><span class="p">,</span> <span class="s2">&quot;2011-Ranger&quot;</span><span class="p">,</span> <span class="s2">&quot;2003-Excursion&quot;</span><span class="p">,</span> <span class="s2">&quot;1997-F350&quot;</span><span class="p">,</span> <span class="s2">&quot;1969-Cadillac&quot;</span><span class="p">]</span>
<span class="p">})</span>

<span class="c1"># Append to List a 2nd Dictionary of key/values</span>
<span class="n">InfoDb</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;FirstName&quot;</span><span class="p">:</span> <span class="s2">&quot;Sunny&quot;</span><span class="p">,</span>
    <span class="s2">&quot;LastName&quot;</span><span class="p">:</span> <span class="s2">&quot;Naidu&quot;</span><span class="p">,</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="s2">&quot;August 2&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Residence&quot;</span><span class="p">:</span> <span class="s2">&quot;Temecula&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="s2">&quot;snaidu@powayusd.com&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Owns_Cars&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;4Runner&quot;</span><span class="p">]</span>
<span class="p">})</span>

<span class="c1"># My information</span>
<span class="n">InfoDb</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;FirstName&quot;</span><span class="p">:</span> <span class="s2">&quot;Arnav&quot;</span><span class="p">,</span>
    <span class="s2">&quot;LastName&quot;</span><span class="p">:</span> <span class="s2">&quot;Kanekar&quot;</span><span class="p">,</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="s2">&quot;July 3&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Residence&quot;</span><span class="p">:</span> <span class="s2">&quot;San Diego&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="s2">&quot;**********@*****.***&quot;</span><span class="p">,</span> <span class="c1"># Censored</span>
    <span class="s2">&quot;Owns_Cars&quot;</span><span class="p">:</span> <span class="s2">&quot;None&quot;</span>
<span class="p">})</span>

<span class="c1"># Using input to add information to the dictionary</span>
<span class="n">InfoDb</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;FirstName&quot;</span><span class="p">:</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What is your first name?&quot;</span><span class="p">),</span>
    <span class="s2">&quot;LastName&quot;</span><span class="p">:</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What is your last name?&quot;</span><span class="p">),</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What is your date of birth(Month, day)?&quot;</span><span class="p">),</span>
    <span class="s2">&quot;Residence&quot;</span><span class="p">:</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Where do you live?&quot;</span><span class="p">),</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What is your email?&quot;</span><span class="p">),</span> 
    <span class="s2">&quot;Owns_Cars&quot;</span><span class="p">:</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What cars do you own?&quot;</span><span class="p">)</span>
<span class="p">})</span>

<span class="c1"># Print the data structure</span>
<span class="nb">print</span><span class="p">(</span><span class="n">InfoDb</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[{&#39;FirstName&#39;: &#39;John&#39;, &#39;LastName&#39;: &#39;Mortensen&#39;, &#39;DOB&#39;: &#39;October 21&#39;, &#39;Residence&#39;: &#39;San Diego&#39;, &#39;Email&#39;: &#39;jmortensen@powayusd.com&#39;, &#39;Owns_Cars&#39;: [&#39;2015-Fusion&#39;, &#39;2011-Ranger&#39;, &#39;2003-Excursion&#39;, &#39;1997-F350&#39;, &#39;1969-Cadillac&#39;]}, {&#39;FirstName&#39;: &#39;Sunny&#39;, &#39;LastName&#39;: &#39;Naidu&#39;, &#39;DOB&#39;: &#39;August 2&#39;, &#39;Residence&#39;: &#39;Temecula&#39;, &#39;Email&#39;: &#39;snaidu@powayusd.com&#39;, &#39;Owns_Cars&#39;: [&#39;4Runner&#39;]}, {&#39;FirstName&#39;: &#39;Arnav&#39;, &#39;LastName&#39;: &#39;Kanekar&#39;, &#39;DOB&#39;: &#39;July 3&#39;, &#39;Residence&#39;: &#39;San Diego&#39;, &#39;Email&#39;: &#39;**********@*****.***&#39;, &#39;Owns_Cars&#39;: &#39;None&#39;}, {&#39;FirstName&#39;: &#39;John&#39;, &#39;LastName&#39;: &#39;Cena&#39;, &#39;DOB&#39;: &#39;April 23&#39;, &#39;Residence&#39;: &#39;Tampa&#39;, &#39;Email&#39;: &#39;johncena@gmail.com&#39;, &#39;Owns_Cars&#39;: &#39;2006 Ford GT, 1970 Plymouth Superbird&#39;}]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="For-Loops">For Loops<a class="anchor-link" href="#For-Loops"> </a></h2><p>Using a for loop to iterate through a list.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sports</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;football&quot;</span><span class="p">,</span> <span class="s2">&quot;track&quot;</span><span class="p">,</span> <span class="s2">&quot;soccer&quot;</span><span class="p">,</span> <span class="s2">&quot;basketball&quot;</span><span class="p">,</span> <span class="s2">&quot;tennis&quot;</span><span class="p">]</span> <span class="c1"># list</span>
<span class="c1"># iterates based on the range, so in this case it will only iterate 5 times</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">5</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">sports</span><span class="p">[</span><span class="n">i</span><span class="p">])</span> <span class="c1"># would not print more than 5 sports, even if list is longer</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>football
track
soccer
basketball
tennis
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="For-Loop-with-an-Index">For Loop with an Index<a class="anchor-link" href="#For-Loop-with-an-Index"> </a></h2><p>Creating a list and using a for loop with indexes to print it. This iterates for every index in the list, making it more powerful and easier to code with.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">cake_flavors</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;chocolate&quot;</span><span class="p">,</span> <span class="s2">&quot;strawberry&quot;</span><span class="p">,</span> <span class="s2">&quot;vanilla&quot;</span><span class="p">]</span> <span class="c1"># List</span>
<span class="c1"># For loop, for index in list</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">cake_flavors</span><span class="p">:</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">i</span><span class="p">)</span> <span class="c1"># Print the flavor</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>chocolate
strawberry
vanilla
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Using-the-While-Loop-and-Inputs">Using the While Loop and Inputs<a class="anchor-link" href="#Using-the-While-Loop-and-Inputs"> </a></h2><p>This demonstrates usage of the while loop. The while loop calls a function as long as a certain condition is met. This is also another example of creating dictionaries using inputs.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">meals</span> <span class="o">=</span> <span class="p">{}</span> <span class="c1"># empty dictionary</span>

<span class="n">length</span> <span class="o">=</span> <span class="mi">4</span>

<span class="c1"># runs as long as there are less than 4 items in the dictionary</span>
<span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">meals</span><span class="p">)</span> <span class="o">&lt;</span> <span class="n">length</span><span class="p">:</span>
    <span class="n">name</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Name a food.&quot;</span><span class="p">)</span>
    <span class="n">rating</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;How would you rate the meal on a scale of 1 - 10?&quot;</span><span class="p">)</span>
    <span class="n">meals</span><span class="p">[</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="n">rating</span> <span class="c1"># determines the key and the value</span>

<span class="nb">print</span><span class="p">(</span><span class="n">meals</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>{&#39;pineapple pizza&#39;: &#39;5&#39;, &#39;chicken alfredo&#39;: &#39;8&#39;, &#39;fried chicken&#39;: &#39;10&#39;, &#39;mango&#39;: &#39;9&#39;}
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Recursion">Recursion<a class="anchor-link" href="#Recursion"> </a></h2><p>Recursive functions are helpful, but can be inefficient since it keeps on recalling the function.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">factorial</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="c1"># defining the function</span>
    <span class="k">if</span> <span class="n">i</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span> <span class="c1"># will not recall function</span>
        <span class="k">return</span> <span class="mi">1</span>
    <span class="k">if</span> <span class="n">i</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span> <span class="c1"># will not recall function</span>
        <span class="k">return</span> <span class="n">i</span>
    <span class="k">if</span> <span class="n">i</span> <span class="o">!=</span> <span class="mi">1</span><span class="p">:</span>
        <span class="k">return</span> <span class="n">i</span> <span class="o">*</span> <span class="n">factorial</span><span class="p">(</span><span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="c1"># recalls the function, but at lesser value</span>

<span class="nb">print</span><span class="p">(</span><span class="n">factorial</span><span class="p">(</span><span class="mi">5</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="n">factorial</span><span class="p">(</span><span class="mi">0</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="n">factorial</span><span class="p">(</span><span class="mi">1</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>120
1
1
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Tools">Tools<a class="anchor-link" href="#Tools"> </a></h2><p>Using other capabilities to organize lists. These are very useful tools.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Reverse-Order">Reverse Order<a class="anchor-link" href="#Reverse-Order"> </a></h1><p>Command to output a list in reverse order.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">countdown</span> <span class="o">=</span> <span class="p">[</span><span class="mi">3</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">1</span><span class="p">]</span> <span class="c1"># New list</span>
<span class="nb">print</span><span class="p">(</span><span class="n">countdown</span><span class="p">)</span>
<span class="n">countdown</span><span class="o">.</span><span class="n">reverse</span><span class="p">()</span> <span class="c1"># Reversing the list</span>
<span class="nb">print</span><span class="p">(</span><span class="n">countdown</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[3, 2, 1]
[1, 2, 3]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This shows that the <code>.reverse()</code> statement is used to reverse a list.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Sort-and-Set">Sort and Set<a class="anchor-link" href="#Sort-and-Set"> </a></h1><p>More functions that can help to alphabetize lists as well as make sure there are no duplicates in the list.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">cake_flavors</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;chocolate&quot;</span><span class="p">,</span> <span class="s2">&quot;strawberry&quot;</span><span class="p">,</span> <span class="s2">&quot;vanilla&quot;</span><span class="p">]</span>
<span class="c1"># Appending multiple items</span>
<span class="n">cake_flavors</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;red velvet&quot;</span><span class="p">)</span>
<span class="n">cake_flavors</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;lemon&quot;</span><span class="p">)</span>
<span class="n">cake_flavors</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;marble&quot;</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">cake_flavors</span><span class="p">)</span> <span class="c1"># Printing the new list</span>

<span class="c1"># Sort function</span>
<span class="n">cake_flavors</span><span class="o">.</span><span class="n">sort</span><span class="p">()</span>
<span class="nb">print</span><span class="p">(</span><span class="n">cake_flavors</span><span class="p">)</span> <span class="c1"># Alphabetized list</span>

<span class="c1"># Appending more flavors</span>
<span class="n">cake_flavors</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;lemon&quot;</span><span class="p">)</span>
<span class="n">cake_flavors</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;german chocolate&quot;</span><span class="p">)</span>
<span class="n">cake_flavors</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;carrot&quot;</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">cake_flavors</span><span class="p">)</span>

<span class="n">cake_flavors</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="n">cake_flavors</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">cake_flavors</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[&#39;chocolate&#39;, &#39;strawberry&#39;, &#39;vanilla&#39;, &#39;red velvet&#39;, &#39;lemon&#39;, &#39;marble&#39;]
[&#39;chocolate&#39;, &#39;lemon&#39;, &#39;marble&#39;, &#39;red velvet&#39;, &#39;strawberry&#39;, &#39;vanilla&#39;]
[&#39;chocolate&#39;, &#39;lemon&#39;, &#39;marble&#39;, &#39;red velvet&#39;, &#39;strawberry&#39;, &#39;vanilla&#39;, &#39;lemon&#39;, &#39;german chocolate&#39;, &#39;carrot&#39;]
{&#39;red velvet&#39;, &#39;carrot&#39;, &#39;marble&#39;, &#39;vanilla&#39;, &#39;german chocolate&#39;, &#39;chocolate&#39;, &#39;lemon&#39;, &#39;strawberry&#39;}
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Showcases the <code>.append()</code>, <code>.sort()</code>, and <code>set()</code>. Append adds a new item to the list, sort puts the list in alphabetical order, and set removes any duplicatte items.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Quiz">Quiz<a class="anchor-link" href="#Quiz"> </a></h2><p>Creating a quiz like last week, except using a list of dictionaries. This makes it easier to store questions and answers as key and value pairs.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">quiz</span> <span class="o">=</span> <span class="p">[]</span> <span class="c1"># empty list</span>

<span class="c1">#variables</span>
<span class="n">question_count</span> <span class="o">=</span> <span class="mi">5</span>
<span class="n">score</span> <span class="o">=</span> <span class="mi">0</span>

<span class="c1"># appending some questions</span>
<span class="n">quiz</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;What type of language is Python&quot;</span> <span class="p">:</span> <span class="s2">&quot;object oriented&quot;</span><span class="p">,</span>
    <span class="s2">&quot;How do you get an output in Python?&quot;</span> <span class="p">:</span> <span class="s2">&quot;print&quot;</span>
<span class="p">})</span>

<span class="n">quiz</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;Is a dictionary a primitive or a collection?&quot;</span> <span class="p">:</span> <span class="s2">&quot;collection&quot;</span><span class="p">,</span>
    <span class="s2">&quot;How do you add more information to a list?&quot;</span> <span class="p">:</span> <span class="s2">&quot;append&quot;</span><span class="p">,</span>
    <span class="s2">&quot;What do you need to call to get the value in a dictionary?&quot;</span> <span class="p">:</span> <span class="s2">&quot;key&quot;</span>
<span class="p">})</span>

<span class="c1"># function to print questions and get answers</span>
<span class="k">def</span> <span class="nf">questioning</span><span class="p">(</span><span class="n">ask</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">ask</span><span class="p">)</span>
    <span class="k">global</span> <span class="n">ans</span>
    <span class="n">ans</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer: &quot;</span> <span class="o">+</span> <span class="n">ans</span><span class="p">)</span>

<span class="c1"># for loop to iterate through the dictionary</span>
<span class="k">for</span> <span class="nb">dict</span> <span class="ow">in</span> <span class="n">quiz</span><span class="p">:</span>
    <span class="k">for</span> <span class="n">question</span><span class="p">,</span> <span class="n">answer</span> <span class="ow">in</span> <span class="nb">dict</span><span class="o">.</span><span class="n">items</span><span class="p">():</span> <span class="c1"># for the key and value pair</span>
        <span class="n">questioning</span><span class="p">(</span><span class="n">question</span><span class="p">)</span> <span class="c1"># calling function</span>
        <span class="k">if</span> <span class="n">ans</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="n">answer</span><span class="p">:</span>
            <span class="n">score</span> <span class="o">+=</span> <span class="mi">1</span>
            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Your answer is correct.&quot;</span><span class="p">)</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You are incorrect.&quot;</span><span class="p">)</span>

<span class="c1"># percentage calculator from last time</span>
<span class="k">def</span> <span class="nf">grade</span><span class="p">(</span><span class="n">sco</span><span class="p">,</span> <span class="n">quests</span><span class="p">):</span> 
    <span class="n">percent</span> <span class="o">=</span> <span class="mi">100</span> <span class="o">*</span> <span class="nb">float</span><span class="p">(</span><span class="n">sco</span><span class="p">)</span><span class="o">/</span><span class="nb">float</span><span class="p">(</span><span class="n">quests</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">percent</span>

<span class="n">quiz_percentage</span> <span class="o">=</span> <span class="n">grade</span><span class="p">(</span><span class="n">score</span><span class="p">,</span> <span class="n">question_count</span><span class="p">)</span> <span class="c1"># Defining variable</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You got &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">score</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; of &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">question_count</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; questions correct.&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Your score is &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">quiz_percentage</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot;%.&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Question: What type of language is Python
Answer: OBJECT ORiented
Your answer is correct.
Question: How do you get an output in Python?
Answer: pRINT
Your answer is correct.
Question: Is a dictionary a primitive or a collection?
Answer: primitive
You are incorrect.
Question: How do you add more information to a list?
Answer: APPEnd
Your answer is correct.
Question: What do you need to call to get the value in a dictionary?
Answer: kEY
Your answer is correct.
You got 4 of 5 questions correct.
Your score is 80.0%.
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
