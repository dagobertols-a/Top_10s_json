# Top_10s_json
Exercise in json

JSON examples and exercise
get familiar with packages for dealing with JSON
study examples with JSON strings and files
work on exercise to be completed and submitted
reference: http://pandas.pydata.org/pandas-docs/stable/io.html#io-json-reader
data source: http://jsonstudio.com/resources/

JSON example, with file
demonstrates reading in a json file as a string and as a table
uses small sample file containing data about projects funded by the World Bank
data source: http://jsonstudio.com/resources/

JSON exercise
Using data in file 'data/world_bank_projects.json' and the techniques demonstrated above,

Find the 10 countries with most projects
Find the top 10 major project themes (using column 'mjtheme_namecode')
In 2. above you will notice that some entries have only the code and the name is missing. Create a dataframe with the missing names filled in.

Summary

Here the ten countries with most projects can be obtained by using a simple value_counts(). In this case the result was:

Republic of Indonesia
People's Republic of China
Socialist Republic of Vietnam
Republic of India
Republic of Yemen
People's Republic of Bangladesh Nepal
Kingdom of Morocco
Africa
Republic of Mozambique

In order to get the top ten major project themes, first, we flatted the column 'mjtheme_namecode' by using json.load and json_normalize. Then, with the help of for loops we filled the empty values in the column name. For this dataset the top ten major project themes are

Environment and natural resources management
Rural development
Human development
Public sector governance
Social protection and risk management
Financial and private sector development
Social dev/gender/inclusion
Trade and integration
Urban development
Economic management
