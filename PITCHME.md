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
<section class="content">

<pre contenteditable="" style="font-size:100%; line-height:1.5" data-gramm_id="d82887c5-17f4-dbe6-f444-ef752e664e34" data-gramm="true" spellcheck="false" data-gramm_editor="true">&lt;ul&gt;
&lt;li id="myID" class="myClass"&gt;item 1&lt;/li&gt;
&lt;li class="myClass"&gt;item 2&lt;/li&gt;
&lt;li&gt;item 3&lt;/li&gt;
&lt;/ul&gt; </pre><grammarly-btn><div style="z-index: 2; opacity: 1; transform: translate(851.25px, 374.25px);" class="_e725ae-textarea_btn _e725ae-show _e725ae-anonymous _e725ae-field_hovered" data-grammarly-reactid=".6"><div class="_e725ae-transform_wrap" data-grammarly-reactid=".6.0"><div title="Protected by Grammarly" class="_e725ae-status" data-grammarly-reactid=".6.0.0">&nbsp;</div></div></div></grammarly-btn>

    <dl class="inline">
      <dt><b class="imp">#</b>myID</dt>
      <dd>ID</dd>
      <dt><b class="imp">.</b>myClass</dt>
      <dd>class</dd>
      <dt class="imp">li</dt>
      <dd>tag name</dd>
    </dl>
  </section>
