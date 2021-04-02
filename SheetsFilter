function viewBacklog()  {
  var spreadsheet = SpreadsheetApp.getActive();
  
  spreadsheet.getActiveSheet().getFilter().remove()
  spreadsheet.getRange('A4:F10000').createFilter();
  
  // Select All
  //var criteria = SpreadsheetApp.newFilterCriteria().setHiddenValues(['']).build()
  
  // Select All BUT...
  //var criteria = SpreadsheetApp.newFilterCriteria().setHiddenValues(['Backlog']).build()
  
  // Select Specifically...
  var criteria = SpreadsheetApp.newFilterCriteria().whenTextEqualToAny(['Backlog']).build();
  
  spreadsheet.getActiveSheet().getFilter().setColumnFilterCriteria(3, criteria);
};
