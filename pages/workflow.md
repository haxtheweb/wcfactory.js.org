<h2>wcf element</h2>
<p>When it's finished, go into the <b>elements/element-name</b>
 directory and run <b><i>yarn start</i>
</b>
. Then open it in a code editor and work within the <b>elements/element-name/src</b>
 directory</p>
<h2>yarn start (monorepo level)</h2>
<p>At the factory level you can also run yarn start which will invoke your storybook to build for previewing locally. Make sure all your elements exist (or that you have some in general). Also, be aware that after you stop your storybook you'll need to run yarn install again. <a href="https://github.com/elmsln/WCFactory/issues/504#issuecomment-484545199">This is a known issue without a real way around it currently.</a>
</p>
