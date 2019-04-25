---
layout: default
---

<!-- Styles -->
<style>
#chartdiv {
  width: 100%;
  height: 650px;
}
</style>

<!-- Resources -->
<script src="https://www.amcharts.com/lib/3/amcharts.js"></script>
<script src="https://www.amcharts.com/lib/3/serial.js"></script>
<script src="https://www.amcharts.com/lib/3/gantt.js"></script>
<script src="https://www.amcharts.com/lib/3/plugins/export/export.min.js"></script>
<link rel="stylesheet" href="https://www.amcharts.com/lib/3/plugins/export/export.css" type="text/css" media="all" />
<script src="https://www.amcharts.com/lib/3/themes/none.js"></script>

<!-- Chart code -->
<script>
var chart = AmCharts.makeChart( "chartdiv", {
  "type": "gantt",
  "theme": "none",
  "marginRight": 70,
  "period": "YYYY",
  "dataDateFormat": "YYYY-MM-DD",
  "columnWidth": 0.5,
  "valueAxis": {
    "type": "date"
  },
  "brightnessStep": 7,
  "graph": {
    "fillAlphas": 1,
    "lineAlpha": 1,
    "lineColor": "#fff",
    "fillAlphas": 0.85,
    "balloonText": "<b>[[category]]</b>:<br />[[start]] ~ [[end]]"
  },
  "rotate": true,
  "categoryField": "category",
  "segmentsField": "segments",
  "startDateField": "start",
  "endDateField": "end",
  "dataProvider": [ {
    "category": "HTML",
    "segments": [ { "start": "2002", "end": "2009", },
                  { "start": "2011", "end": "2017", },
                  { "start": "2018", "end": "2019", } ]
  }, {
    "category": "CSS",
    "segments": [ { "start": "2004", "end": "2017", },
                  { "start": "2019", "end": "2019", } ]
  }, {
    "category": "JavaScript",
    "segments": [ { "start": "2004", "end": "2017", },
                  { "start": "2019", "end": "2019", } ]
  }, {
    "category": "VBScript",
    "segments": [ { "start": "2004", "end": "2009", },
                  { "start": "2014", "end": "2017", } ]
  }, {
    "category": "XML",
    "segments": [ { "start": "2004", "end": "2017", } ]
  }, {
    "category": "BAT",
    "segments": [ { "start": "2015", "end": "2017", } ]
  }, {
    "category": "Visual Basic",
    "segments": [ { "start": "2006", "end": "2007", },
                  { "start": "2014", "end": "2017", } ]
  }, {
    "category": "ASP.Net",
    "segments": [ { "start": "2006", "end": "2017", } ]
  }, {
    "category": "AJAX.Net",
    "segments": [ { "start": "2008", "end": "2013", } ]
  }, {
    "category": "C#",
    "segments": [ { "start": "2006", "end": "2019", } ]
  }, {
    "category": "JSON",
    "segments": [ { "start": "2009", "end": "2010", },
                  { "start": "2017", "end": "2019", } ]
  }, {
    "category": "ASP.Net MVC",
    "segments": [ { "start": "2009", "end": "2010", },
                  { "start": "2015", "end": "2018", } ]
  }, {
    "category": "ASP.Net Core",
    "segments": [ { "start": "2018", "end": "2019", } ]
  }, {
    "category": "REST API",
    "segments": [ { "start": "2018", "end": "2019", } ]
  }, {
    "category": "TypeScript",
    "segments": [ { "start": "2019", "end": "2019", } ]
  }, {
    "category": "Angular-CLI",
    "segments": [ { "start": "2019", "end": "2019", } ]
  }, {
    "category": "Java",
    "segments": [ { "start": "2009", "end": "2010", },
                  { "start": "2016", "end": "2017", } ]
  }, {
    "category": "WPF",
    "segments": [ { "start": "2009", "end": "2010", } ]
  }, {
    "category": "WCF",
    "segments": [ { "start": "2010", "end": "2017", } ]
  }, {
    "category": "SourceSafe",
    "segments": [ { "start": "2006", "end": "2007", },
                  { "start": "2009", "end": "2010", } ]
  }, {
    "category": "ClearCase",
    "segments": [ { "start": "2006", "end": "2007", },
                  { "start": "2009", "end": "2010", },
                  { "start": "2011", "end": "2017", } ]
  }, {
    "category": "ClearQuest",
    "segments": [ { "start": "2006", "end": "2007", },
                  { "start": "2009", "end": "2010", },
                  { "start": "2011", "end": "2017", } ]
  }, {
    "category": "SVN",
    "segments": [ { "start": "2009", "end": "2010", } ]
  }, {
    "category": "PVCS",
    "segments": [ { "start": "2010", "end": "2013", } ]
  }, {
    "category": "GIT",
    "segments": [ { "start": "2017", "end": "2019", } ]
  }, {
    "category": "MDB",
    "segments": [ { "start": "2002", "end": "2004", } ]
  }, {
    "category": "MS SQL",
    "segments": [ { "start": "2003", "end": "2019", } ]
  }, {
    "category": "Oracle",
    "segments": [ { "start": "2014", "end": "2018", } ]
  }, {
    "category": "Mongo",
    "segments": [ { "start": "2017", "end": "2019", } ]
  }, {
    "category": "CosmosDB",
    "segments": [ { "start": "2019", "end": "2019", } ]
  } ],
  "valueScrollbar": {
    "autoGridCount": true
  },
  "chartCursor": {
    "cursorColor": "#55bb76",
    "valueBalloonsEnabled": false,
    "cursorAlpha": 0,
    "valueLineAlpha": 0.5,
    "valueLineBalloonEnabled": true,
    "valueLineEnabled": true,
    "zoomable": false,
    "valueZoomable": true
  },
  "export": {
    "enabled": true
  }
} );
</script>

<!-- HTML -->
<div id="chartdiv"></div>
