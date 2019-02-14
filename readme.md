## Création d'un thème enfant.
Dans un nouveau dossier dans le dossier des thèmes:

- créer 2 fichiers
- 1 style.css
- 1 function.php

## style.css


Theme Name:   Theme enfant Child

Template:     twentynineteen

Description:  Twenty Nineteen Child Theme

Author:       Justine Telmann

Author URI:   Ness

Version:      1.0.0

License:      GNU General Public License v3 or later

License URI:  http://www.gnu.org/licenses/gpl-3.0.html

Text Domain:  twenty-nineteen-child


copier/coller les code ci-dessus en modifier au minimum les 3 premieres lignes

## function.php
```PHP
<?php
add_action( 'wp_enqueue_scripts', 'my_theme_enqueue_styles' );
function my_theme_enqueue_styles() {
$parent_style = 'parent-style'; // This is 'twentynineteen-style' for the Twenty nineteen theme.
wp_enqueue_style( $parent_style, get_template_directory_uri() . '/style.css' );
wp_enqueue_style( 'child-style', get_stylesheet_directory_uri() . '/style.css', array( $parent_style ));
}
?>
```
Permet de modifier la structure HTML.

## installation 

aller dans thème et activé le thème enfant.


### Anglais

In the new folder :

- create 2 files
- 1 style.css
- 1 function.php

## style.css

Theme Name:   Theme enfant Child

Template:     twentynineteen

Description:  Twenty Nineteen Child Theme

Author:       Justine Telmann

Author URI:   Ness

Version:      1.0.0

License:      GNU General Public License v3 or later

License URI:  http://www.gnu.org/licenses/gpl-3.0.html

Text Domain:  twenty-nineteen-child

copy / paste the code above modifying at least the first 3 lines

## function.php

```PHP
<?php
add_action( 'wp_enqueue_scripts', 'my_theme_enqueue_styles' );
function my_theme_enqueue_styles() {
$parent_style = 'parent-style'; // This is 'twentynineteen-style' for the Twenty nineteen theme.
wp_enqueue_style( $parent_style, get_template_directory_uri() . '/style.css' );
wp_enqueue_style( 'child-style', get_stylesheet_directory_uri() . '/style.css', array( $parent_style ));
}
?>
```

Permet de modifier la structure HTML.

Edit the HTML structure.

## installation

go into theme and activate the child theme.
