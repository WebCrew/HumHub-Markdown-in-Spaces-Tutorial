# HumHub-Markdown-in-Spaces-Tutorial
With this tutorial you will be able to have Markdown Syntrax support in all of HumHub CMS **Spaces and Comments**. I can understand the performance implications of doing this on the server side. However, there aren't **any of those concerns** if we process the Markdown on the client side, so all is fine.
***

##Tutorial

-  Upload the JS folder with the humhub_markdown.js to your theme folder (the theme you are using)
-  open views/layouts/head.php with a code editor like Sublime or Notepad++ and integrate the following code snippet:

`<!-- MARKDOWN IN SPACES -->	
<?php $this->registerJsFile( $this->theme->getBaseUrl().'/js/humhub_markdown.js', ['position'=>\yii\web\View::POS_END]); ?>`
-  now save the head.php and upload it again back to your theme folder
-  juhuuu, now you are ready to use Markdown in Spaces and Comments


***

###Extra

If you want a bit more color and nice style with your messages and comments then you can use this....

-  open HumHUb/themes/yourtheme/css/theme.css and paste at the very end the following code:

-  `
.panel-body strong {
    font-weight: bold;
    color: rgb(173, 39, 8);
    font-size: 15px;
    font-family: "PT Sans";
}
`
-  `
code {
    color: #1cc1f5;
    background-color: #1d2024;
    border: 1px solid #000;
}
`
- good luck and have fun using it :)

***


###You can use only the following Markdown tags

- list style: `- your text here, or + your text here, or 1. your text here` 
- bold text: `**your text**`
- italic text: `*your text* or _your text_`
- titles (H3,H4): `### Your H3 title, or #### Your H4 title `
- horizontal rules: `three underscores ___ or three asterisks ***`


***
###Important Note 

Do **not use** other Markdown tags as mentioned, otherwise the website **stops loading**!!!
***

##Autors

-  The original autor of the humhub_markdown.js is: https://community.humhub.com/u/joeworkman/
-  Andreas Holzer / WebCrew https://github.com/WebCrew
