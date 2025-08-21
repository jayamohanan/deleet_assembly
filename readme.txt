What this HTML does

This HTML is the index.html of a static website hosted on GitHub Pages. Along with this index.html file, other geopackage files are provided; these files contain the boundary data and other attributes of administrative divisions in Kerala, like districts and assemblies.
'assembly_V15.geojson' contains the boundaries of all the assemblies in Kerala
'district_V15.geojson', which contains the boundaries of all the 14 districts in Kerala. 

The main field/attribute that can be used to search rows(assemblies/districts) is "Name". The "Name" field in the assembly and district GeoJSON, respectively, contains the names of all the assemblies and districts of Kerala.

Purpose of Static Website: Selectively draw boundaries as requested.
For every type of boundary, i.e. geojson file, there will be a separate panel that contains the input fields to select that kind of boundary. The user can select the boundary to be shown using the input panel. Each panel contains:
An input field where name(or names separated by commas) can be entered(which searches against the "Name" field in the respective geojoson(or parsed data)), this input field is preferred to be auto-suggestive, and
Color picker to select the color of boundaries drawn, the default color should be black, and 
A transparency slider that controls the transparency of the fill of boundaries(each boundary is drawn as an outline and a fill for that outline ), the default transparency should be the maximum value, and 
A “Draw” button, when clicked, draws the boundary based on inputs -Name, color, and transparency.
A “Clear” button that erases all boundaries drawn of its kind(e.g., it erases all district boundaries that are drawn if the “Clear” button of the district panel is clicked)

Show multiple boundaries simultaneously. Sample case: 
Step 1: I enter an assembly name and click the “Draw” button for the assembly, and the requested assembly should be drawn. 
Step 2: I enter a district name and click the ”Draw” button for the district; the asked district should be drawn along with the previously drawn district.
Step 3: I click the “Clear” button in the district panel, and now the district map drawn previously is removed, with only the assembly outline remaining.




HTML Code Standards
Every time you edit/create the HTML file, make sure you increment the version number(if editing)/add a version number(if newly creating)
During runtime, the version number shown at the top right always overlays everything. Also, in the HTML code, the version number should be displayed as a comment so that I can easily understand the version number without searching between code lines.


