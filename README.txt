CSS FEEDBACK

1) Structure

>>>>> FEEDBACK I GOT
This is the only concern left. You've been so great about addressing the others! Please take this additional effort to fix this as it is required for the project.

It's important that you not mix type and class selectors. Please follow this one guideline in order to make sure your code is consistent and follows the guideline. It is more performant and more readable. As it says in the Style Guide:

    Avoid qualifying ID and class names with type selectors.

    Unless necessary (for example, with helper classes), do not use element names in conjunction with IDs or classes. Avoiding unnecessary ancestor selectors is useful for performance reasons.

Wherever you've used an element name selector (img, li, a, etc.), please make sure to create a new class and apply it to that element locally.

For example, .nav-link instead of .nav > li > a. It is more concise and better for performance.

Please avoid ancestor selectors. Refer directly to expressive classes assigned locally to the element you wish to style.





>>>>> WHAT I DID?

I took out the old code, added classes on my HTML and created a new CSS for the classes, but I would really like to have a feedback about the code.
Why can’t I use the same structure from Bootstrap, because this one is exactly the same, if they use and I just want to change the way it looks, what is the problem there? I can’t get it!
I always believed in order to overwrite the old code would be the best to follow the same sintax in the new CSS you are adding.


.nav > li {
	margin: 0 25px 0 0;
	padding: 10px;
}
.nav > li {
	border-top: 6px solid transparent;
	margin: 0 25px 0 0;
	padding: 10px;
}

.nav > li > a,
.nav > li > a:hover {
	color: #000;
	text-transform: uppercase;
	font-weight: bold;
	font-size: 16px;
	background-color: transparent;
	padding: 0;
}

.nav > li > a:hover {
	color: #e6001c;
}

.nav > li:hover,
.nav > li.active {
	border-top: 6px solid #e6001c;
	color: #e6001c;
	background-color: transparent;
}

.nav > li.active > a:hover,
.nav > li.active > a {
	color: #e6001c;
	background-color: transparent;
}

a.dropdown-toggle .glyphicon {
	font-size: 10px;
	color: #000 !important;
}

.nav > li > a:hover,
.nav > li > a:focus,
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus,
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
	background-color: transparent;
}

.dropdown-menu > li > a,
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus,
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
	padding: 5px 10px 2px 10px;
	border: 0;
	font-weight: normal;
	text-transform: none;
	background-color: transparent;
}

.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
	color: #e6001c;
	background-image: none !important;
}

