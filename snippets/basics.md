# Basics

## Hide some content from search

Hiding content from search is useful for some widgets, modules or templates

```
<!-- indexer::stop -->
<p>Content to hide from search</p>
<!-- indexer::continue -->
```
## Change CSS of Backend

Useful for customising the backend for clients or hiding some elements. insert the path leading to your css. Add this snippet to your initconfig.php, located at sytem/config/.

```
if(TL_MODE == 'BE') $GLOBALS['TL_CSS'][] = 'files/theme/be.css';
```
