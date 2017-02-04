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
<object data="https://raw.githubusercontent.com/blambodhar/CSS/master/files/00_basics.html"></object>

