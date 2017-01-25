# HumHub-Markdown-in-Spaces-Tutorial
With this tutorial you will be able to have Markdown Syntrax support in all of HumHub CMS **Spaces and Comments**.

##Tutorial

-  Upload the JS folder with the humhub_markdown.js to your theme folder (the theme you are using)
-  open views/layouts/head.php with a code editor like Sublime or Notepad++ and integrate the following code snippet:

`<!-- MARKDOWN IN SPACES -->	
<?php $this->registerJsFile( $this->theme->getBaseUrl().'/js/humhub_markdown.js', ['position'=>\yii\web\View::POS_END]); ?>`
-  now save the head.php and upload it again back to your theme folder
-  juhuuu, now you are ready to use Markdown in Spaces and Comments

##Markdown Cheatsheet

-  here you can find a cheatsheet for Markdown code: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
-  NOTE: The H1 and H2 Tags are not working because of SEO. 
-  Also do not use Markdown code to integrate Links, it is better to just paste it as always (the HumHub default way)

##Autors

-  The original autor of the humhub_markdown.js is: https://community.humhub.com/u/joeworkman/
-  Andreas Holzer / WebCrew https://github.com/WebCrew
