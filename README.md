# megamenu-js-bs4
The only Megamenu jQuery plugin + Bootstrap4 you ever want. 

Updated: November 21, 2019 

![Image of the Megamenu-JS](https://github.com/OrangeWacko/megamenu-js/blob/master/mega-menu-js.jpg)

## This MegamenuJS is inspired by the  (https://github.com/marioloncarek/megamenu-js) from @marioloncarek.


## Features
- Bootstrap4 support
- Cross-browser compatibility
- Smart - knows when to show megamenu, and when to show a normal dropdown
- 100% responsive, works on all devices
- Seamless wordpress integration
- Super fast
- Uses jquery animations (IE8 compatible)
- Easy to use
- Uses ionicons
- Super small
- Free to use and abuse (MIT licence)


## Demos
Download and open index.html **or:**
#### Live Demo
Live demo on Codepen:
[megamenu.js demo](https://codepen.io/orange_wacko/pen/wvvZaBK)



## Installation
1) This version uses Bootstrap4 CSS for the Demo index.html, so include the stylesheet from CDN: 
```
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
```
1.1) Copy CSS from **style.css** or **style.less**

1.2) megamenu.js uses [ionicons](http://ionicons.com/) for icons, so include stylesheet in your project: 
```
<link rel="stylesheet" href="css/ionicons.min.css">
```

2) Include jquery just before closing body tag `</body>`
```
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
```

3) Include **megamenu.js** **below** jquery
```
<script src="js/megamenu.js"></script>
```

4) Wrap your menus HTML in megamenu.js wrappers and see the magic :)

```
<div class="menu-container">
        <div class="menu">
                <ul>
                  <li><a>Link</a></li>
                  <li>
                    <a>Mega Link</a>
                    <div class="mega-menu"><!-- Whatever, basic html menu(lists)! Dont worry megamenu.js will know --></div>
                  </li>
                </ul>
        </div>
    </div>
```


## Usage and jQuery explanation
This version uses Bootstrap4 to build HTML content inside the Mega-menu HTML containers. 


## Wordpress integration
Use the custom HTML5 Walker to build the structure of your Wordpress menu that matches the Megamenu-JS example above:

**1)** In your functions.php add these lines ([taken from HTML5blank by @toddmotto](https://github.com/toddmotto/html5blank))

That customizes the menu from everything Wordpress has added and from this point the menu is like you are doing a static version.

**2)** Then simply wrap the wordpress menu with megamenu.js wrappers!

```
<div class="menu-container">
    <div class="menu">
      <?php wp_nav_menu(); ?>
    </div>
</div>
```

## Made with (thanks)
- [Bootstrap4](https://getbootstrap.com/)
- [Jquery](http://jquery.com/)
- [Ionicons](http://ionicons.com/)
- [Codepen](http://codepen.io)
- [Wordpress](https://codex.wordpress.org/)
- [HTML5Blank](https://github.com/toddmotto/html5blank)
- [Stackoverflow](stackoverflow.com)
