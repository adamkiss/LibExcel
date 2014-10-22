# Excel for ProcessWire v0.0.1

This is a ProcessWire wrapper for the [PHPExcel](https://github.com/PHPOffice/PHPExcel). In addition to including the PHPExcel, it also includes few functions for generating very simple excel tables (think: outputting a two dimensional array into excel file).

## Usage

``` php
  // example: usage from other modules
  $excel = $this->modules->get('LibExcel'); 
  
  //Let's use 'simple mode' to export simple table
  $excel->table_columns = [15, 20, 15]; //set column width
  $excel->table_headers = ['Column 1', 'Column 2', 'Column 3'];
  $excel->table_data = $prepared_table_data; //two dimensional array
  $excel->render('browser', 'excel-filename.xls'); //output to browser

  // alternatively, use PHPExcel object for advanced things
  $php_excel = $excel->get_php_excel();
```

## License

The wrapper itself is licensed under [WTFPL](https://github.com/adamkiss/LibraryOffice/blob/master/LICENSE).

[PHPExcel](https://github.com/PHPOffice/PHPExcel) is licensed under [LGPL (GNU LESSER GENERAL PUBLIC LICENSE)](https://github.com/PHPOffice/PHPExcel/blob/master/license.md).