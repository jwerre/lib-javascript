# ImageCharts.ChartApi

All URIs are relative to *https://image-charts.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getChart**](ChartApi.md#getChart) | **GET** /chart | Image-Charts API


<a name="getChart"></a>
# **getChart**
> &#39;String&#39; getChart(cht, chd, chs, opts)

Image-Charts API

Image-charts

### Example
```javascript
var ImageCharts = require('image_charts');

var apiInstance = new ImageCharts.ChartApi();

var cht = "cht_example"; // String | chart type

var chd = "chd_example"; // String | chart data

var chs = "chs_example"; // String | chart size

var opts = { 
  'chds': "chds_example", // String | text format custom scaling
  'chxr': "chxr_example", // String | axis range
  'chxp': "chxp_example", // String | axis label positions
  'chof': ".png", // String | output fake format
  'chdl': "", // String | text for each series, to display in the legend
  'chdls': "000000", // String | chart legend text and style
  'chg': "chg_example", // String | grid lines
  'chco': "F56991,FF9F80,FFC48C,D1F2A5,EFFAB4", // String | series colors
  'chtt': "", // String | chart title
  'chts': "", // String | chart title colors and font size
  'chxt': "chxt_example", // String | axis to apply labels to
  'chxl': "", // String | custom axis labels
  'chxs': "chxs_example", // String | color, size, alignment, and formatting of axis labels
  'chm': "", // String | line fills
  'chls': "", // String | line thickness and solid/dashed style
  'chl': "", // String | pie chart labels
  'chma': "chma_example", // String | chart margins
  'chdlp': "b", // String | (upcoming)
  'chf': "bg,s,FFFFFF", // String | Background Fills
  'chbh': "10", // String | Bar Width and Spacing. (not supported)  You can optionally specify custom values for bar widths and spacing between bars and groups. You can only specify one set of width values for all bars. If you don't specify chbh, all bars will be 23 pixels wide, which means that the end bars can be clipped if the total bar + space width is wider than the chart width.
  'chan': "chan_example", // String | gif configuration
  'chli': "chli_example", // String | doughnut chart inside label
  'icac': "icac_example", // String | image-charts enterprise `account_id`
  'ichm': "ichm_example", // String | HMAC-SHA256 signature
  'icwt': false // Boolean | Force watermark display even if the chart was signed with an enterprise account
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getChart(cht, chd, chs, opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cht** | **String**| chart type | 
 **chd** | **String**| chart data | 
 **chs** | **String**| chart size | 
 **chds** | **String**| text format custom scaling | [optional] 
 **chxr** | **String**| axis range | [optional] 
 **chxp** | **String**| axis label positions | [optional] 
 **chof** | **String**| output fake format | [optional] [default to .png]
 **chdl** | **String**| text for each series, to display in the legend | [optional] [default to ]
 **chdls** | **String**| chart legend text and style | [optional] [default to 000000]
 **chg** | **String**| grid lines | [optional] 
 **chco** | **String**| series colors | [optional] [default to F56991,FF9F80,FFC48C,D1F2A5,EFFAB4]
 **chtt** | **String**| chart title | [optional] [default to ]
 **chts** | **String**| chart title colors and font size | [optional] [default to ]
 **chxt** | **String**| axis to apply labels to | [optional] 
 **chxl** | **String**| custom axis labels | [optional] [default to ]
 **chxs** | **String**| color, size, alignment, and formatting of axis labels | [optional] 
 **chm** | **String**| line fills | [optional] [default to ]
 **chls** | **String**| line thickness and solid/dashed style | [optional] [default to ]
 **chl** | **String**| pie chart labels | [optional] [default to ]
 **chma** | **String**| chart margins | [optional] 
 **chdlp** | **String**| (upcoming) | [optional] [default to b]
 **chf** | **String**| Background Fills | [optional] [default to bg,s,FFFFFF]
 **chbh** | **String**| Bar Width and Spacing. (not supported)  You can optionally specify custom values for bar widths and spacing between bars and groups. You can only specify one set of width values for all bars. If you don&#39;t specify chbh, all bars will be 23 pixels wide, which means that the end bars can be clipped if the total bar + space width is wider than the chart width. | [optional] [default to 10]
 **chan** | **String**| gif configuration | [optional] 
 **chli** | **String**| doughnut chart inside label | [optional] 
 **icac** | **String**| image-charts enterprise &#x60;account_id&#x60; | [optional] 
 **ichm** | **String**| HMAC-SHA256 signature | [optional] 
 **icwt** | **Boolean**| Force watermark display even if the chart was signed with an enterprise account | [optional] [default to false]

### Return type

**&#39;String&#39;**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/png, application/gif

