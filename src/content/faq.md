---
title: FAQ
---
<h2>There's a lot going on here, can't you make this easier?</h2>
<p>We're working on a UI that helps in running the commands but organizing and managing a company library / brand for your organization is tricky. Our tooling reduces issues in setup as much as it can (though we'll keep trying to make it easier!)</p>
<h2>Do I have to use Polymer to use this?</h2>
<p>While we do use Polymer CLI this tool is able to build and analyze any web component regardless of library.</p>
<h2>What commands do I need to install this?</h2>
<code-sample copy-clipboard-button="copy-clipboard-button" style="width: 50%;">  <template preserve-content="preserve-content">yarn global add @wcfactory/cli
yarn global add polymer-cli
yarn global add lerna</template>
</code-sample>
<h2>Do I need to publish this to NPM?</h2>
<p>Yes and No. We highly recommend publishing your elements to NPM as part of your build process and quality assurance. That doesn't always make sense to get off the ground so here's what you can do to get "building" without NPM.</p>
<code-sample style="width: 100%;">  <template preserve-content="preserve-content"># assuming your factory name is ourelements
# also assuming you have your company installed in ~/Documents/company
wcf build
# answer the prompts, assuming name of the build is mybuild
# this will fail but it's ok
cd ~/Documents/company/builds/mybuild
ln -s ../../factories/ourelements/node_modules/
polymer build
# Now you'll have the buidl satisfied without publishing to NPM</template>
</code-sample>
