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


how does developer like me konw about this <div class="note custom-note">

Step 1: Start from your DITA source
<p>This is a paragraph.</p>

<note type="tip">
  Always validate your XML.
</note>

<ul>
  <li>First</li>
  <li>Second</li>
</ul>

Step 2: Build with html5 and inspect the output

Inspect the generated HTML

Build your DITA map with the default html5 transtype.

Open the output in a browser.

Right-click → Inspect → check the DOM.

You’ll see exactly what DITA-OT emitted.

Example for a plain <note>:
<div class="note">
  <span class="note__title">Note</span>
  <div class="note__body">
    <p>Some important information.</p>
  </div>
</div>
