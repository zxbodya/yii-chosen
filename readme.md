Chosen usage instructions
===

1. Checkout source code to your project, for example to ext.chosen.

2. Use it, as any input widget, for example:
<pre>
    $this->widget('ext.chosen.Chosen',array(
        'name' => 'inputName', // input name
        'value' => '2', // selection
        'data' => array( // list of select options
            '1'=>'Option 1',
            '2'=>'Option 2',
            '3'=>'Option 3',
            '4'=>'Option 4',
        ),
    ));
</pre>

3. Also you can use it like CHtml helper:
    1. In config/main.php add:
    'import' => array(
        'ext.chosen.Chosen',
    ),

    2. Use
        Chosen::dropDownList($name, $select, $data, $htmlOptions);
        Chosen::activeDropDownList($model, $attribute, $data, $htmlOptions);
        Chosen::multiSelect($name, $select, $data, $htmlOptions);
        Chosen::activeMultiSelect($model, $attribute, $data, $htmlOptions);