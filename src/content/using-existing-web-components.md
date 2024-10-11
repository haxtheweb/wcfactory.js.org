---
title: Reusing web components
---
<p>So you want to leverage all that goodness from web components [dot] org huh? Awesome! There's a minor thing you need to do differently from typical yarn repos you might be used to.</p>
<p>Because this is a monorepo and we're optimizing for file space, you need to always do installations from the monorepo (factory) root. Here's the workflow for adding elements from webcomponents.org / other npm repos</p>
<ul><li>find something you like, like @haxtheweb/code-editor</li>
<li>go to the element you want to use this in and add it manually to the package.json (<b><i>factories/my-factory/elements/my-element/package.json</i>
</b>
)</li>

<li>go to the factory floor / monorepo root (<i><b>factories/my-factory</b>
</i>
)</li>
<li>run <i><b>yarn install</b>
</i>
</li>
<li>Profit</li>
</ul>
<a11y-gif-player src="https://media2.giphy.com/media/67ThRZlYBvibtdF9JH/giphy.gif" src-without-animation="https://media2.giphy.com/media/67ThRZlYBvibtdF9JH/480w_s.jpg" alt="bugs bunny counting money by WB Looney Tunes" resource="#d0403aa6-2eff-1bfa-fdec" prefix="oer:http://oerschema.org/ schema:http://schema.org/ dc:http://purl.org/dc/terms/ foaf:http://xmlns.com/foaf/0.1/ cc:http://creativecommons.org/ns# bib:http://bib.schema.org " style="width: 25%;"></a11y-gif-player>
<p><span style="caret-color: rgb(0, 0, 0);">This is a little annoying (<i><b>ehhh what's up doc</b>
</i>
) for sure but VS Code plugins help ensure that you add things to the package.json of the correct version in the dependencies block. All of our element library implementations have a dependencies and devDependencies block automatically.</span></p>
