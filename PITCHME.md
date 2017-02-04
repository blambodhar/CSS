#HSLIDE

# CSS3
<span class="primary"><strong>blambodhar</strong></span> - 02.06.2017

#HSLIDE

## Introduction to CSS (Cascading Style Sheets)
- Styles and Stylesheets <!-- .element: class="fragment" -->
- Selectors <!-- .element: class="fragment" -->
- Inheritence and Cascading styles <!-- .element: class="fragment" -->
- CSS Box Model <!-- .element: class="fragment" -->
- CSS Media Queries <!-- .element: class="fragment" -->

#HSLIDE

## Styles and Stylesheets
- Inline Styles defined using style attribute <!-- .element: class="fragment" -->
- Style Element defined in head <!-- .element: class="fragment" -->
- External Stylesheet file defined in head <!-- .element: class="fragment" -->

#VSLIDE
### Inline Styles
<pre style="background:#002240;color:#fff"><span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">p</span> <span style="color:#9effff">style</span>=<span style="color:#3ad900">"</span>color: red;<span style="color:#3ad900">"</span><span style="color:#e1efff">></span></span> This is a paragraph <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
<span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
</pre>

#VSLIDE

### Using Style Element
<pre style="background:#002240;color:#fff"><span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">style</span><span style="color:#e1efff">></span></span>
        p {
          font-size: 16px;
        }
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">style</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">p</span> style="color: red;"<span style="color:#e1efff">></span></span> This is a paragraph <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
<span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
</pre>

#VSLIDE

### External Stylesheet file
<pre style="background:#002240;color:#fff"><span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">link</span> <span style="color:#9effff">rel</span>=<span style="color:#3ad900">"</span>stylesheet<span style="color:#3ad900">"</span> <span style="color:#9effff">href</span>=<span style="color:#3ad900">"</span>styles.css<span style="color:#3ad900">"</span><span style="color:#e1efff">/></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span> This is a paragraph <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
<span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>

<p> style.css file contents </p>
<span style="color:#9effff">p</span> <span style="color:#e1efff">{</span>
   <span style="color:#9df39f">font-size</span><span style="color:#e1efff">:</span> <span style="color:#edf080">16<span style="color:#ff9d00">px</span></span><span style="color:#e1efff">;</span>
}
</pre>

#HSLIDE
## Selectors
- Basic Selectors
<pre style="background:#002240;color:#fff"><span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">ul</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">li</span> <span style="color:#9effff">id</span><span style="color:#e1efff">=</span><span style="color:#3ad900">"</span><span style="color:#3ad900">myID</span><span style="color:#3ad900">"</span> <span style="color:#9effff">class</span>=<span style="color:#3ad900">"</span>myClass<span style="color:#3ad900">"</span><span style="color:#e1efff">></span></span>item 1<span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">li</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">li</span> <span style="color:#9effff">class</span>=<span style="color:#3ad900">"</span>myClass<span style="color:#3ad900">"</span><span style="color:#e1efff">></span></span>item 2<span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">li</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">li</span><span style="color:#e1efff">></span></span>item 3<span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">li</span><span style="color:#e1efff">></span></span>
<span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">ul</span><span style="color:#e1efff">></span></span> 
</pre>

#VSLIDE
- Relational Selectors
<section class="content future" style="text-shadow: rgba(0, 0, 0, 0.2) 0px 2px 5px; margin: 20px 30px 0px; display: block; overflow: hidden; top: 79.5px;" aria-hidden="true">
  <div class="ex right" style="
  float: right;
  width: 200px;
  text-align: left;
  font-size: 80%;
  padding: 10px 20px;
  background: rgba(255, 255, 255, 0.6);
  -moz-border-radius: 8px;
  border-radius: 8px;
  border: 1px solid #fff;
">
    <ol>
      <li>item 1</li>
      <li>item 2</li>
      <li>item 3
        <ul>
          <li>item a</li>
          <li>item b</li>
          <li>item c</li>
        </ul>
      </li>
      <li class="hasaclass">hasaclass</li>
      <li>item 5</li>
      <li>item 6</li>
      <li>item 7</li>
    </ol>
  </div>
  <dl style="
    margin-right: 250px;
    display: block;
    font-size: 75%;
">
    <dt style="
  font-weight: bold;
  margin-top: 0.5em;
  background-color: #ccc;
  display: inline-block;
  margin-bottom: 2px;
  clear: both;
"><span onclick="hasaclass('ul li');">ul li</span>, <br><span onclick="hasaclass('ol li');">ol li</span></dt>
    <dd>descendant selector<br>
      matches nested &lt;li&gt;s
    </dd>
    <dt onclick="hasaclass('ol > li');">ol&nbsp;&gt;&nbsp;li</dt>
    <dd><em>child selector</em>&nbsp;<br>
    matches &lt;li&gt;s in &lt;ol&gt; but not nested &lt;ul&gt;</dd>
    <dt onclick="hasaclass('li.hasaclass + li');">li.hasaclass +&nbsp;li</dt>
    <dd><em>adjacent sibling</em>&nbsp;</dd>
    <dt onclick="hasaclass('li.hasaclass ~ li');"><strong class="new">NEW&nbsp; </strong><span style="background-color:#eee; padding:3px 20px; position:relative; left: 22px; margin-left: -20px;">(IE7+)</span><br>
    li.hasaclass ~&nbsp;li</dt>
    <dd><em>general sibling selector</em><br>
    matches later siblings, but not nested.</dd>
  </dl>
</section>
  

#VSLIDE
- <a target="_blank" href='http://codepen.io/blambodh/full/jyKMXW/'>Try Basic Selector</a> 

