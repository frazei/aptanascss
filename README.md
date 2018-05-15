<h1>aptanascss</h1>

That's my personal best way to manage the sass/scss compilation within Appcelerator Studio.<br />
It should work in every IDE derived from Eclipse (like Titanium/Appcelerator Studio).<br />
The only prerequisite:
<pre>
$ sudo gem install sass
</pre>
Many tutorials/how-to that I've read are using compass or ant to achieve one simple task: to compile automatically a sass/scss file every time I save it.<br />
Fortunately this can be done using the "external builder" feature inside Eclipse.<br />
<h2>How to do it the easy way:</h2>
<ol>
<li>Clone the repository
<pre>
$ git clone https://github.com/frazei/aptanascss.git
</pre></li>
<li>Link the binary to your path
<pre>
$ ln -s ~/Documents/GitHub/aptanascss/aptanascss /usr/local/bin
$ chmod +x /usr/local/bin/aptanascss
</pre></li>
<li>Go to the root of the project and then..
<pre>
$ mkdir .externalToolBuilders
$ ln -s ~/Documents/GitHub/aptanascss/Aptana\ Scss.launch .externalToolBuilders
</pre></li>
<li>Enable the external builder: select the project > Properties (&#8984; + i) > Builders > Check "Aptana Scss" > Click "Apply and Close"</li>
</ol>
<br />
Repeat step 3 and 4 for every project.<br />
