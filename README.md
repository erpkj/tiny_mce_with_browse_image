To change upload directory 
============================
Go to tiny_mce_with_browse_image\plugins\ajaxfilemanager\inc\config.tinymce.php

Find below script:

define('CONFIG_SYS_DEFAULT_PATH', '../uploaded/'); //accept relative path only

define('CONFIG_SYS_ROOT_PATH', '../uploaded/');	//accept relative path only


If file browser popup is not opening
=====================================
Go to tiny_mce_with_browse_image\index.php

Find below script:


  var ajaxfilemanagerurl = "plugins/ajaxfilemanager/ajaxfilemanager.php"; //check file path 
		
  url: "plugins/ajaxfilemanager/ajaxfilemanager.php", //check file path 
               
