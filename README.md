# A web-responsive wedding website 

<p>A very good method to keep your guests informed during the most spcial day of your life - the big wedding. A simple webpage offering your guest information like: locations, program, gifts, a question &amp; answers section and finnaly the contacts infos.</p>

<p>This website was made in CodeBerry Programming  school during practice with help of the HTML and CSS programming languages, if you want to see a live version acces this page: <a href="https://negrut112.github.io/wedding-website/">https://negrut112.github.io/wedding-website/</a>.</p>
    
<br>
    
<img src="https://i.imgur.com/ILXmTcU.png">

## HTML

<p>First step was to establish the framework: header, footer and different sections.</p>
<p>I will give an example of a location section where it will take part: the ceremony, photos session and the party.</p>

<pre><code>&lt;section class=“locations”&gt;<br>
&lt;h2&gt;Locations&lt;/h2&gt;<br>
&lt;div class=“info”&gt;<br>
&lt;h3&gt;Ceremony&lt;/h3&gt;<br>
&lt;img src=&quot;<a href="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-ceremony.png">https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-ceremony.png</a>&quot; alt=“Ceremony”&gt;<br>
&lt;div&gt;St. Nicholas Church&lt;/div&gt;<br>
&lt;div&gt;2 Trinity Square, Bucharest&lt;/div&gt;<br>
&lt;/div&gt;</p>
&lt;div class=&quot;info&quot;&gt;
    &lt;h3&gt;Photos&lt;/h3&gt;
    &lt;img src=&quot;https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-photoshoot.png&quot; alt=&quot;Photoshoot&quot;&gt;
    &lt;div&gt;Liberty Bastion&lt;/div&gt;
    &lt;div&gt;23 Wisdom Road, Bucharest&lt;/div&gt;
  &lt;/div&gt;
  &lt;div class=&quot;info&quot;&gt;
    &lt;h3&gt;Party&lt;/h3&gt;
    &lt;img src=&quot;https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-party.png&quot; alt=&quot;Party&quot;&gt;
    &lt;div&gt;Heaven Lounge&lt;/div&gt;
    &lt;div&gt;14 Fairy Street, Bucharest&lt;/div&gt;
  &lt;/div&gt;
&lt;/section&gt;
</code></pre>

## CSS

<p>Next step was to add some style for almost each element from html, but starting first with a Meyer reset that will remove default styling.I did this adding <a href="https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.css">https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.css</a>&quot;&gt;this external link to HTML head tags.</p>

<p>Examples of styling:</p>

<pre><code>body {<br>
background: url(’<a href="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-background.png">https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-background.png</a>') repeat center;<br>
font-family: ‘Libre Baskerville’, serif;<br>
font-size: 1.125rem;<br>
line-height: 1.5;<br>
color: #444349;<br>
}</p>
<p>.text {<br>
margin: 0 auto;<br>
padding: .625rem;<br>
color: hsla(0,0%,100%,.9);<br>
background: hsla(100,0%,0%,.5);<br>
}</p>
<p>footer {<br>
height: 10vh;<br>
width: 100vw;<br>
background-color: #606060;<br>
color: #fff;<br>
font-family: ‘Muli’, sans-serif;<br>
display: table;<br>
text-align: center;<br>
font-size: .875rem;<br>
}</code></pre>

<p>Media queries styling:</p>

<p>@media (min-width: 768px) {</p>
<p>.cover {<br>
background: url(’<a href="https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-cover.jpg">https://orange.codeberryschool.com/content/images/project-assets/wedding-landing-cover.jpg</a>') no-repeat center/cover;<br>
}</p>
<p>.text {<br>
padding: 1.25rem;<br>
border-radius: 4px;<br>
width: 50%;<br>
}</p>
<p>.text h1 {<br>
font-size: 7rem;<br>
}</p>
<pre><code>.info {
display: inline-block;
width: 30%;
padding: 1.5rem;
margin: .5rem;
</code></pre>
<p>}</p>
<p>.info::after {<br>
display: none;<br>
}</p>
<p>.question-group {<br>
display: inline-block;<br>
width: 30%;<br>
vertical-align: top;<br>
padding: 1.5rem;<br>
margin: .5rem;<br>
}</p>
<p>.program-wrapper {<br>
width: 30vw;<br>
margin: 0 auto;<br>
}</p>
<p>.question-group::after {<br>
display: none;<br>
}</p>
<p>.question-group h3 {<br>
text-align: left;<br>
}</p>
<p>footer {<br>
min-height: 7vh;<br>
}</p>
<p>}</p>
