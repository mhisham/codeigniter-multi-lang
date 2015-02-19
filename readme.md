#Multi-language in Codeigniter as a Hook

This document describe how to do multi-language supoort in codeigniter 2.x using hooks .

#installation
Please put files as in folder structure for this git repository and do this modification to config.php file .

Add this code 
```$config['short_language']	= 'en';
 $config['system_lang'] = array ('ar'=>'arabic','en'=>'english');```

This code add support to two language (Arabic and English) you can add as many as you want and define it's codes as you wish i.e (ara for arabic ,ru for Russian or whatever ) .

With no extra configuration , you just need to create language folders i.e(arabic,english) inside `application/languages` folder and add `general_lang.php` for each one .

#Example
To show word `hello` in booth languages , you have to create this key inside booth files `general_lang.php` inside arabic folder and english folder 

```$lang['hello'] = 'Hello'; This for english folder
$lang['hello'] = 'مرحبا'; This for arabic folder```

And at view,or controller or even model you can call `echo lang('hello');`

##That's all
Please feel free to ask for any modification or report bugs <br/>
Thanks.
