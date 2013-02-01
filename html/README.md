# HTML Coding Style

_**Note:** The examples in this style guide uses css methods to help identify tags and structure_

## Basic HTML structure

The first thing to note is the use of spacing for the element hierarchy, this is an indent of 2 spaces. Using spaces helps with consistent code formatting in other editors, especially when it comes to alignments (such as form inputs and imgs with several attribute values).

The base doctype for any site is the HTML5 doctype(`<!doctype html>`) with a little modernizr action to fix legacy browsers

### Head contents

### Commenting

A generous use of commenting is used throughout the document, to signpost scripts and imports as well as making it easy to keep track of the element tree and where they close.

_Example 1:_
    
    <head>
      <title>Site Title</title> 
      
      <!-- Inclusion of the Google hosted jQuery library -->
      <script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.0/jquery.min.js">
      </script>
    </head>
    
_Example 2:_

    <div class="contentContainer">
    
      <!-- Site content body -->
    
    </div><!-- /.contentContainer -->


## HTML5 element structure and layout.

### Header and hgroup elements

#### Header

`<header>` used to wrap the nav and top section of the site as well as any sections of `<article>` to consulate assoicated article meta data (including the use of the `<time>` element.

_Example 1:_

    <header class="mainHeader">
      <nav>
        <!-- Site Navigation -->
      </nav>
    </header><!-- /.mainHeader -->
      
_Example 2:_
       
    <article class="post">
      <header>
        <!-- Article date/meta information -->
      </header>
      
      <!-- Article body -->
    </article><!-- /.post -->

#### hgroup    

The `<hgroup>` element is used to group a set of headings, for example a sites title and accompanying subtitle.

_Example:_

    <header class="mainHeader">
      <hgroup>
        <h1><!-- Site Title --></h1>
        <h2><!-- Subtitle --></h2>
      </hgroup>  
    </header><!-- /.mainHeader -->

### Article element

### Section element

`<section>` elements used for blocks of content that begin with a heading, often contained within an `<article>`. 

_Example:_

    <article class="post">
      <!-- Article headings(see above), introduction etc... -->
      
      <section>
        <h2><!-- Section Heading --></h2>
        <!-- Section content -->
      </section>
      
      <!-- Continuing sections of article -->
    </article><!-- /.post -->

A good tool to use to find out if you are using the `<section>` correctly on your site is to use the [HTML 5 Outliner](http://gsnedders.html5.org/outliner/). It will break the site down into it's respective section with their headings, if it comes back with "Untitled Section" then a section has been incorrectly defined (_You may see "Untitled Section" returned from `<nav>` or `<aside>` sections_).

### Summary element

### Figure and figcaption elements

### Aside element

### Footer element