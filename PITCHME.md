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
<pre style="background:#002240;color:#fff"><span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">p</span> <span style="color:#9effff">style</span>=<span style="color:#3ad900">"</span>color: red;<span style="color:#3ad900">"</span><span style="color:#e1efff">></span></span> This is a paragraph <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
<span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
</pre>
#VSLIDE
- Style Element defined in head <!-- .element: class="fragment" -->
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
- External Stylesheet file defined in head <!-- .element: class="fragment" -->
<pre style="background:#002240;color:#fff"><span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">link</span> <span style="color:#9effff">rel</span>=<span style="color:#3ad900">"</span>stylesheet<span style="color:#3ad900">"</span> <span style="color:#9effff">href</span>=<span style="color:#3ad900">"</span>styles.css<span style="color:#3ad900">"</span><span style="color:#e1efff">/></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">head</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
     <span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span> This is a paragraph <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span>
   <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">body</span><span style="color:#e1efff">></span></span>
<span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">html</span><span style="color:#e1efff">></span></span>
</pre>
<br/>
<pre style="background:#002240;color:#fff"><span style="color:#9effff"><span style="color:#e1efff">&lt;</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span> style.css <span style="color:#9effff"><span style="color:#e1efff">&lt;/</span><span style="color:#9effff">p</span><span style="color:#e1efff">></span></span>


p {
   font-size: 16px;
}
</pre>
