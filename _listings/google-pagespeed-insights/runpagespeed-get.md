---
swagger: "2.0"
info:
  title: PageSpeed Insights
  description: Analyzes the performance of a web page and provides tailored suggestions
    to make that page faster.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /pagespeedonline/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /runPagespeed:
    get:
      summary: Run PageSpeed Analysis
      description: Runs PageSpeed analysis on the page at the specified URL, and returns
        PageSpeed scores, a list of suggestions to make that page faster, and other
        information
      operationId: pagespeedonline.pagespeedapi.runpagespeed
      parameters:
      - in: query
        name: filter_third_party_resources
        description: Indicates if third party resources should be filtered out before
          PageSpeed analysis
      - in: query
        name: locale
        description: The locale used to localize formatted results
      - in: query
        name: rule
        description: A PageSpeed rule to run; if none are given, all rules are run
      - in: query
        name: screenshot
        description: Indicates if binary data containing a screenshot should be included
      - in: query
        name: strategy
        description: The analysis strategy to use
      - in: query
        name: url
        description: The URL to fetch and analyze
      responses:
        200:
          description: OK
      tags:
      - pagespeed analysis
definitions:
  PagespeedApiFormatStringV2:
    properties:
      args:
        description: This is a default description.
        type: parameters
      format:
        description: This is a default description.
        type: parameters
  PagespeedApiImageV2:
    properties:
      data:
        description: This is a default description.
        type: parameters
      height:
        description: This is a default description.
        type: parameters
      key:
        description: This is a default description.
        type: parameters
      mime_type:
        description: This is a default description.
        type: parameters
      page_rect:
        description: This is a default description.
        type: parameters
      width:
        description: This is a default description.
        type: parameters
  Result:
    properties:
      formattedResults:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      invalidRules:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      pageStats:
        description: This is a default description.
        type: parameters
      responseCode:
        description: This is a default description.
        type: parameters
      ruleGroups:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
      version:
        description: This is a default description.
        type: parameters
x-collection-name: Google PageSpeed Insights
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---