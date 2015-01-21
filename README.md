# CSS3-Bar-Graphs

 main.css is the main style sheet. It is located in styles directory. 
 
 File is divided in the following sections:

BAR GRAPH - classes describing the overall graph size and background, used fonts, links and default lists styles,
Y-AXIS LABELS - classes describing alignment of y-axis text labels,
X-AXIS LABELS - classes describing alignment of x-axis text labels,
GRAPH LABEL - main graph label style,
GRAPH - graph area and classes describing graph grid style,
BARS COMMON - common set of styles for data bars including bar width, bar label styles and bars positions from the left side of the graph,
BLUE BAR to RED BAR - bars color styles,
HOVERS - bars hover styles.
HTML Structure
<!-- css bar graph -->
<div class="css_bar_graph">
			
	<!-- y_axis labels -->
	<ul class="y_axis">
		<li>...</li>
		<li>...</li>
		<li>...</li>
		[...]
	</ul>
			
	<!-- x_axis labels -->
	<ul class="x_axis">
		<li>...</li>
		<li>...</li>
		<li>...</li>
		[...]
	</ul>
			
	<!-- graph -->
	<div class="graph">
		<!-- grid -->
		<ul class="grid">
			<li>...</li>
			<li>...</li>
			<li>...</li>
			[...]
			<li class="bottom">...</li>
		</ul>
				
		<!-- bars -->
		<!-- 250px = 100% -->
		<ul>
			<li class="bar nr_1 blue" style="height: 125px;"><div class="top"></div><div class="bottom"></div><span>...</span></li>
			<li class="bar nr_2 blue" style="height: 225px;"><div class="top"></div><div class="bottom"></div><span>...</span></li>
			<li class="bar nr_3 blue" style="height: 75px;"><div class="top"></div><div class="bottom"></div><span>...</span></li>
			[...]
		</ul>	
	</div>
			
	<!-- graph label -->
	<div class="label"><span>...</span>...</div>
		
</div>
The entire graph is contained within css_bar_graph class. Within there is in order: y_axis list with y-axis text labels and x_axis list with horizontal x-axis text labels.

Each data bar is a single list element described by bar, nr_1 ... nr_n, blue ... red classes. bar is a base bar class; nr_n where "n" is a number - is a class which positions bar element from the left side of the graph; blue is a color style for bar element. Bar heights are determined by inline height value - style="height: 75px;"; next there is top and bottom class for top and bottom bar circles and within span there is a place for bar label.

Last elemenet within css_bar_graph class is a graph label.
