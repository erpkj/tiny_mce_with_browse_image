To change upload directory 
============================
Go to tiny_mce_with_browse_image\plugins\ajaxfilemanager\inc\config.tinymce.php

Find below script:
define('CONFIG_SYS_DEFAULT_PATH', '../uploaded/'); //accept relative path only
define('CONFIG_SYS_ROOT_PATH', '../uploaded/');	//accept relative path only


If file browser popup is not opening
=====================================
function ajaxfilemanager(field_name, url, type, win) {
  		var ajaxfilemanagerurl = "plugins/ajaxfilemanager/ajaxfilemanager.php"; //check file path 
			switch (type) {
				case "image":
					break;
				case "media":
					break;
				case "flash": 
					break;
				case "file":
					break;
				default:
					return false;
			}
            tinyMCE.activeEditor.windowManager.open({
                url: "plugins/ajaxfilemanager/ajaxfilemanager.php", //check file path 
                width: 782,
                height: 440,
                inline : "yes",
                close_previous : "no"
            },{
                window : win,
                input : field_name
            });
		}
