# Extensions

# Listing all available variables of a template

```
<pre><?= $this->showTemplateVars(); ?></pre>
```
Read more about showing variables on [contaowiki.org](http://de.contaowiki.org/Template_Variablen_anzeigen)

# Getting database values

```
<?php 
$arrResult = array();
$objResult = \Database::getInstance()->execute('SELECT data1, data2 FROM tl_yourtable'); 
$arrResult = $objResult->fetchAllAssoc();
?>

<?php foreach($arrResult as $result) : ?>
<div>
 <p><?= $result['data1'] ?></p>
 <img src="<?= $result['data2'] ?>" alt=""/>
</div>
<?php endforeach; ?>
```

Gets datas from given database table. Useful for simply displaying them or for further processing.