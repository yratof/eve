---
layout: post
title: "The missing gutter"
author: "Andrew Lazarus"
date: 2015-10-31 14:49:03
published: true
tags:
- gutter
- columns
- grid systems
- design
meta:
  svg_header: '<svg xmlns="http://www.w3.org/2000/svg" width="225.8" height="175" viewBox="0 0 225.8 175"><style>.st0{fill:#ED1C24;} .st1{fill:none;stroke:#ED1C24;stroke-width:5;stroke-miterlimit:10;} .st2{fill:none;stroke:#ED1C24;stroke-width:5;stroke-miterlimit:10;stroke-dasharray:12.1538,12.1538;} .st3{fill:none;stroke:#000000;stroke-width:5;stroke-miterlimit:10;}</style><path id="XMLID_48_" class="st0" d="M65.4 2.5h10.7v170H65.4z"/><path id="XMLID_47_" class="st0" d="M102.2 2.5h10.7v170h-10.7z"/><path id="XMLID_46_" class="st0" d="M139 2.5h10.7v170H139z"/><path id="XMLID_45_" class="st0" d="M175.8 2.5h10.7v170h-10.7z"/><g id="XMLID_39_"><g id="XMLID_41_"><path id="XMLID_44_" class="st1" d="M212.6 2.5h10.7v6"/><path id="XMLID_43_" class="st2" d="M223.3 20.7v139.7"/><path id="XMLID_42_" class="st1" d="M223.3 166.5v6h-10.7"/></g></g><path id="XMLID_38_" class="st3" d="M39.3 2.5h36.8v170H39.3z"/><path id="XMLID_37_" class="st0" d="M28.6 2.5h10.7v170H28.6z"/><path id="XMLID_36_" class="st3" d="M2.5 2.5h36.8v170H2.5z"/><path id="XMLID_35_" class="st3" d="M76.1 2.5h36.8v170H76.1z"/><path id="XMLID_34_" class="st3" d="M112.9 2.5h36.8v170h-36.8z"/><path id="XMLID_28_" class="st3" d="M149.7 2.5h36.8v170h-36.8z"/><path id="XMLID_27_" class="st3" d="M186.5 2.5h26.1v170h-26.1z"/></svg>'
  tl;dr: 'Add 3/4 of the gutter to the width of your column to account for the missing gutter'
author:
  email: yratof@gmail.com
  display_name: Andrew
  first_name: Andrew
  last_name: Lazarus
  
---

## The problem.

Designers skip the last gutter and grid systems don't understand this. This makes life difficult when wanting to make things 1/3rds with a gutter that is fixed.

## The solution.

Don't bother with grid systems to try and solve this issue. Just do some very simple math but with some mental calculations.

Here are some examples. 

#### 4 elements, each spanning 3 columns

This means we have 3 gutters being used and the last one is missing. Because there are 3 out of 4 gutters showing, you should add 75% of a gutter's width to each column. 

Sounds weird right? Here's the code

	
	$gutter: 1.5rem;

	/* Three columns, Four elements */
	.three_columns{
		width: calc(25% - #{$gutter * 0.75});
	}

	/* Four columns, three elements */
	.three_columns{
		width: calc(33% - #{$gutter * 0.66});
	}

The way it works is you say "there are only 5 gutters, there should be 6. So I'm going to get 5/6th of the gutter and add that to the width of every column with a gutter."

## The mixin.
	
	// Strip unit function https://css-tricks.com/snippets/sass/strip-unit-function/
	@function strip-unit($number) {
	  @if type-of($number) == 'number' and not unitless($number) {
	    @return $number / ($number * 0 + 1);
	  }
	  @return $number;
	}

	/*
	 * @param: $width - width in percent
	 * @param: $gutter - gutter in rem or px
	 * @param: $last - if this is the last item 
	 * @usage: missing_gutter_column_calculation(50%, 1.875rem)
	 */
	@mixin missing_gutter_column_calculation( $width, $gutter, $last: false){
		// Percentage stripped
		$fraction: 100 / strip-unit($width);
		$three_quarters: ($fraction - 1) / $fraction;
		
		width: calc(#{$width} - #{$gutter * $three_quarters});
		.no-csscalc & { width: ($width - (strip-unit($gutter) * $three_quarters)) }
		
		// If this is the last item
		@if ($last == false){ margin-right: $gutter; }
	}