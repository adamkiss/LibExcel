# Excel for ProcessWire v0.0.0

This is a ProcessWire wrapper for the [PHPExcel](https://github.com/PHPOffice/PHPExcel). In addition to including the PHPExcel, it also includes few functions for generating very simple excel tables (think: outputting a two dimensional array into excel file).

## Usage

``` php
  // example: usage from other modules
  $excel = $this->modules->get('LibraryExcel'); 
  
  // …your code, $excel is now your new PHPExcel document

  // alternatively, switch to simple mode
  $excel->set_simple_mode();
```

## License

The wrapper itself is licensed under [WTFPL](https://github.com/adamkiss/LibraryOffice/blob/master/LICENSE).

[PHPExcel](https://github.com/PHPOffice/PHPExcel) is licensed under [LGPL (GNU LESSER GENERAL PUBLIC LICENSE)](https://github.com/PHPOffice/PHPExcel/blob/master/license.md).