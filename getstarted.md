---
layout: page
title: Exploratory Data Analysis
subtitle:
bigimg: /img/list.jpg
---

EDA process mainly contains three aspects: 

1. analysis from **users** aspect; 
2. analysis from **products** aspect; 
3. analysis from **users * products** aspect



1.First let's start analyzing from **users** aspect, considering below features:


## a.	How many orders did they make?


<div class='tableauPlaceholder' id='viz1556060299271' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;D1&#47;D1-Orders&#47;useridorderid&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='D1-Orders&#47;useridorderid' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;D1&#47;D1-Orders&#47;useridorderid&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>
<script type='text/javascript'> var divElement = document.getElementById('viz1556060299271');var vizElement = divElement.getElementsByTagName('object')[0];vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';var scriptElement = document.createElement('script');scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

## b.	How many distinct users?

<div class='tableauPlaceholder' id='viz1556060915623' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;di&#47;distinct_15560608602340&#47;distinct&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='distinct_15560608602340&#47;distinct' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;di&#47;distinct_15560608602340&#47;distinct&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>var divElement = document.getElementById('viz1556060915623');var vizElement = divElement.getElementsByTagName('object')[0];vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';var scriptElement = document.createElement('script');scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; vizElement.parentNode.insertBefore(scriptElement, vizElement);</script>

## c.	How many orders in each weekday?

<div class='tableauPlaceholder' id='viz1556061911453' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;di&#47;distinct_15560608602340&#47;day_of_week&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='distinct_15560608602340&#47;day_of_week' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;di&#47;distinct_15560608602340&#47;day_of_week&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>
<script type='text/javascript'>var divElement = document.getElementById('viz1556061911453');var vizElement = divElement.getElementsByTagName('object')[0];vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';var scriptElement = document.createElement('script');scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; vizElement.parentNode.insertBefore(scriptElement, vizElement);</script>


## d. How many orders in each hour of a day?

<div class='tableauPlaceholder' id='viz1556235133376' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;GF&#47;GFJ4KP88J&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='shared&#47;GFJ4KP88J' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;GF&#47;GFJ4KP88J&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>
<script type='text/javascript'>var divElement = document.getElementById('viz1556235133376');var vizElement = divElement.getElementsByTagName('object')[0];if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1000px';vizElement.style.height='827px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1000px';vizElement.style.height='827px';} else { vizElement.style.width='100%';vizElement.style.height='727px';}var scriptElement = document.createElement('script');scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; vizElement.parentNode.insertBefore(scriptElement, vizElement);</script>


## e.	Reorder vs Not Reorder?

<div class='tableauPlaceholder' id='viz1556244397374' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;D3&#47;D3-Reorder&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='D3-Reorder&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;D3&#47;D3-Reorder&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>var divElement = document.getElementById('viz1556244397374');var vizElement = divElement.getElementsByTagName('object')[0];if ( divElement.offsetWidth > 800 ) { vizElement.style.width='700px';vizElement.style.height='627px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='700px';vizElement.style.height='627px';} else { vizElement.style.width='100%';vizElement.style.height='727px';}var scriptElement = document.createElement('script');scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);</script>

## f.	How many orders were given after how many days?

<div class='tableauPlaceholder' id='viz1556244181196' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;NY&#47;NYX7TSHWN&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='shared&#47;NYX7TSHWN' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;NY&#47;NYX7TSHWN&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div> 
<script type='text/javascript'>var divElement = document.getElementById('viz1556244181196');var vizElement = divElement.getElementsByTagName('object')[0];if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1000px';vizElement.style.height='627px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1000px';vizElement.style.height='627px';} else { vizElement.style.width='100%';vizElement.style.height='727px';}var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                 vizElement.parentNode.insertBefore(scriptElement, vizElement);</script>

## g. How many products are there in all baskets of the user at total?
<div class='tableauPlaceholder' id='viz1556247112738' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;D3&#47;D3-Reorder&#47;Sheet5&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='D3-Reorder&#47;Sheet5' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;D3&#47;D3-Reorder&#47;Sheet5&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>
<script type='text/javascript'>var divElement = document.getElementById('viz1556247112738');var vizElement = divElement.getElementsByTagName('object')[0];vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';var scriptElement = document.createElement('script');scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; vizElement.parentNode.insertBefore(scriptElement, vizElement);              </script>

### 1. Fork the Beautiful Jekyll repository 

Fork the [repository](https://github.com/daattali/beautiful-jekyll) by clicking the Fork button on the top right corner in GitHub.

### 2. Rename the repository to `yourusername.github.io`

This will create a GitHub User page ready with the **Beautiful Jekyll** template that will be available at http://yourusername.github.io (sometimes it takes a few minutes).

### 3. Customize settings

Edit the `_config.yml` file to change all the settings to reflect your site.  The settings in the file are fairly self-explanatory and I added comments inside the file to help you further.  Every time you make a change to any file, your website will get rebuilt and should be updated at `yourusername.github.io` within a minute.

<div class="get-started-wrap">
  <a class="btn btn-success btn-lg get-started-btn" href="https://github.com/daattali/beautiful-jekyll#readme">Get Started!</a>
</div>
