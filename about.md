---
title: About
layout: page
---
![Profile Image]({{ site.url }}/{{ site.picture }})

<p>
Senior Software Engineer at Block with 14+ years of experience crafting scalable software solutions. Proven track record in distributed systems, microservices architecture, and cloud computing across fintech, healthcare, and enterprise domains.
</p>

<p>I'm passionate about continuous learning, building resilient systems, and solving complex technical challenges. I believe in writing clean, maintainable code and leading through collaboration and knowledge sharing.</p>

<h2>Core Competencies</h2>

<b>Distributed Systems:</b> Building and scaling microservices architectures with high availability<br />
<b>Backend Development:</b> Java, Kotlin, Python, Ruby, and Scala for enterprise applications<br />
<b>Cloud & Infrastructure:</b> AWS, Docker, Kubernetes, and cloud-native solutions<br />
<b>System Architecture:</b> Designing resilient, scalable systems for fintech and enterprise domains<br />

<!--
<ul class="skill-list">
	<li>HTML5 and CSS3</li>
	<li>Responsive (Mobile First)</li>
	<li>Javascript (ES6)</li>
	<li>AngularJS</li>
	<li>Scrum</li>
	<li>TDD and Continuous Integration</li>
</ul>
-->
<style>
@import url(https://fonts.googleapis.com/css?family=Lato:400,900);  /* <-- Just for the demo, Yes I like pretty fonts... */

.boxes .square {
    float:left;
    position: relative;
    width: 20%;
    padding-bottom :20%; /* = width for a 1:1 aspect ratio */
    background-color:#1E1E1E;
    overflow:hidden;
}

.boxes .content {
    position:absolute;
    height:90%; /* = 100% - 2*5% padding */
    width:90%; /* = 100% - 2*5% padding */
    padding: 5%;
    
}
.boxes .table{
    display:table;
    width:100%;
    height:100%;
}
.boxes .table-cell{
    display:table-cell;
    vertical-align:middle;
}
/*  For list */
.boxes ul{
    text-align:left;
    margin:5% 0 0;
    padding:0;
    list-style-position:inside;
}
.boxes li{
    margin: 0 0 0 5%;
    padding:0;
}

.boxes {
    font-size:15px;
    font-family: 'Lato',verdana, sans-serif;
    color: #fff;
    text-align:center;
    background:#ECECEC;
}

.boxes p{
    margin:0;
    padding:0;
    text-align:left;
}

.numbers{
    font-weight:900;
    font-size:25px;
}

#bottom {
    clear:both;
    margin:0 1.66%;
    width:89.68%;
    padding: 3.5%;
    background-color:#1E1E1E;
    color: #fff;
}
#bottom p{
    text-align:center;
    line-height:2em;
}
#bottom a{
    color: #000;
    text-decoration:none;
    border:1px solid #000;
    padding:10px 20px 12px;
    line-height:70px;
    background:#ccc;
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
}

#bottom a:hover{
    background:#ECECEC;
    border:1px solid #fff;
}
</style>

<h2 style="text-align:center">Selected Technical Skills</h2>
<div class="boxes">
{% for a in site.skills %}
{% assign skillsize = site.skillcolors | size %}
{% assign c_index =  forloop.index | modulo: skillsize  %}
<div class="square" style="background-color:{{ site.skillcolors[c_index] }}" >
    <div class="content">
        <div class="table">
            <div class="table-cell numbers" >
                    {{ a }} 
            </div>
        </div>
    </div>
</div>
{% endfor %}
<div style="clear:both"> </div>
</div>

<!--
<h2>Projects</h2>

<ul>
	<li><a href="https://github.com/">Lorem Lorem</a></li>
	<li><a href="https://github.com/">Ipsum Dolor</a></li>
	<li><a href="https://github.com/">Dolor Lorem</a></li>
</ul>
-->
