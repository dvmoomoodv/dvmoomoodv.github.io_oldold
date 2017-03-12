---
layout: minimal
title: "About me"
permalink: /about/index.html
description: "Some description about Lorem Ipsum..."
---

<script src="https://apis.google.com/js/api.js"></script>
<script>
<!-- Spreadsheet: http://spreadsheets.google.com/feeds/ /
o13394135408524254648.240766968415752635
/
od6
/public/values -->

function start() {
 gapi.client.init({
	 'apiKey': 'AIzaSyCOOLdapQgwJ-zjD-j6jlZfuRgDrTjZslI',
	 'discoveryDocs': ['https://www.googleapis.com/discovery/v1/apis/translate/v2/rest'],
 }).then(function() {
	 return gapi.client.language.translations.list({
		 q: 'hello world',
		 source: 'en',
		 target: 'de',
	 });
 }).then(function(response) {
	 console.log(response.result.data.translations[0].translatedText);
 }, function(reason) {
	 console.log('Error: ' + reason.result.error.message);
 });
};
gapi.load('client', start);


$(function(){

	<!-- $.ajax({url: "https://spreadsheets.google.com/feeds/list/key/1IzUNOwFAh6dyNvzMHkLUYtDTU-Rs6ufwwyjDQ2EDcD8/private/basic", success: function(result){ -->
	$.ajax({url: "https://sheets.googleapis.com/v4/spreadsheets/1IzUNOwFAh6dyNvzMHkLUYtDTU-Rs6ufwwyjDQ2EDcD8", success: function(result){
	        $("#div1").html(result);
  }});


});



</script>

<iframe src="https://docs.google.com/spreadsheets/d/1IzUNOwFAh6dyNvzMHkLUYtDTU-Rs6ufwwyjDQ2EDcD8/pubhtml?widget=true&amp;headers=false"></iframe>


<img itemprop="image" class="img-rounded" src="/assets/img/blog-author.jpg" alt="Willian Justen">

<h2>About Me</h2>

<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>


<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>


<h2>Skills</h2>

<ul class="skill-list">
	<li>HTML - Jade - Haml - Erb</li>
	<li>Design Responsivo (Mobile First)</li>
	<li>CSS (Stylus, Sass, Less)</li>
	<li>Css Frameworks (Bootstrap, Foundation)</li>
	<li>Javascript (Design Patterns, Testes)</li>
	<li>NodeJS</li>
	<li>AngularJS - ReactJS</li>
	<li>Grunt - Gulp - Yeoman</li>
	<li>Git</li>
	<li>PHP</li>
	<li>Python</li>
	<li>MySQL - MongoDB</li>
	<li>Scrum and Kanban</li>
	<li>TDD e Continuous Integration</li>
</ul>

<h2>Projetos</h2>

<ul>
	<li><a href="https://github.com/">Lorem Lorem</a></li>
	<li><a href="https://github.com/">Ipsum Dolor</a></li>
	<li><a href="https://github.com/">Dolor Lorem</a></li>
</ul>
