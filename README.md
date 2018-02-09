# jScroll Contao component

[![Latest Stable Version](https://poser.pugx.org/heimrichhannot-contao-components/jscroll/v/stable)](https://packagist.org/packages/heimrichhannot-contao-components/jscroll)
[![Total Downloads](https://poser.pugx.org/heimrichhannot-contao-components/jscroll/downloads)](https://packagist.org/packages/heimrichhannot-contao-components/jscroll)

Shim repository for [jScroll](https://github.com/pklauzinski/jscroll) as [Contao Component](https://github.com/contao-components/installer).


## Install

```
composer require heimrichhannot-contao-components/jscroll
```


## Config

Add the following to your config (keep keys to prevent double integration):

### Contao 4

```
$GLOBALS['TL_JAVASCRIPT']['huh_components_jscroll'] = 'assets/jscroll/dist/jquery.jscroll.min.js|static';
```

### Contao 3

```
$GLOBALS['TL_JAVASCRIPT']['huh_components_jscroll'] = 'assets/components/jscroll/dist/jquery.jscroll.min.js|static';
```


## Internal
 
Update Library:

```
svn export https://github.com/pklauzinski/jscroll.git/trunk/jquery.jscroll.js ./dist --force
/usr/bin/yui-compressor dist/jquery.jscroll.js -o dist/jquery.jscroll.min.js
```