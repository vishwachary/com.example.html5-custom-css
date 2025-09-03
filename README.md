Adding custom headers and footers
You add a custom header to include a publication title, company logo, or other common branding elements in HTML output. A custom footer can also be added with copyright information, legal boilerplate, or other fine print.

step 1

create custom plugin folder

step 2

create footer xml file

create header xml file

step 3

create ant build file

step 4

create plugin.xml file

Coomand to run , with temp folder outside your dia dir

.\dita-ot-3.7.4\bin\dita --clean.temp=no --debug --input C:\\Ddrive\\1_DocEng\\Sample-DITA-OT-Project\\test_source_sample_map_topics\\sample.ditamap -format html5-custom-css -o MyTestHtmlOutput --temp C:\Ddrive\my-temp > dita_output1_new2.log 2>&1

.\dita-ot-3.7.4\bin\dita -i mymap.ditamap -f html5-custom-css -o out-html5 --temp C:\Ddrive\my-temp


