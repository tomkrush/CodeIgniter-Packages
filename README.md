# Usage

These classes have only been confirmed to work in CodeIgniter 2.0.2. Place My_Router.php and My_Loader.php in *application/core*.

Add array to config/config.php

$config['packages'] = array(
	APPPATH.'third_party/example'
);

Add modification to autoload.php on line 40.

$CI =& get_instance();
$autoload['packages'] = $CI->config->item('packages');