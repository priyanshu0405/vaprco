<script>
	export let segment;
</script>

<style>
	/*nav {
		border-bottom: 1px solid rgba(255,62,0,0.1);
		font-weight: 300;
		padding: 0 1em;
	}

	ul {
		margin: 0;
		padding: 0;
	}*/

	/* clearfix */
	/*ul::after {
		content: '';
		display: block;
		clear: both;
	}

	
	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -1px;
		transition-property: width;
		transition-duration: 1s;
	}
	[aria-current]:hover{
		width:fit-content;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}*/

	/*button
	{
    	padding: 10px 10px;
    	font-size: 20px;
    	text-align: center;
    	cursor: pointer;
    	outline: none;
    	color: #fff;
		background-color: black;
    	border: none;
    	border-radius: 0.5px;
	}

	button:hover 
	{
		background-color: rgb(255,62,0);
	}*/

	/*nav {
  width: 80%;
  margin: 0 auto;
  background: #fff;
  padding: 50px 0;
  box-shadow: 0px 5px 0px #dedede;
}*/
nav ul {
  list-style: none;
  text-align: right;
}
nav ul li {
	font-size: 1.6rem;
  display: inline-block;
}
nav ul li a {
  display: block;
  padding: 15px;
  text-decoration: none;
  color:#fff;
  font-weight: 300;
  text-transform: uppercase;
  margin: 0 10px;
}
nav ul li a,
nav ul li a:after,
nav ul li a:before {
  transition: all .5s;
}
nav ul li a:hover {
  color: darkgreen;
}

nav.fill ul li a {
  position: relative;
}

nav.fill ul li a:after {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  margin: auto;
  width: 0%;
  content: '.';
  color: transparent;
  height: 1px;
}

nav.fill ul li a {
  transition: all 2s;
}

nav.fill ul li a:after {
  text-align: right;
  content: '.';
  margin: 0;
  opacity: 0;
}
nav.fill ul li a:hover {
  z-index: 1;
}
nav.fill ul li a:hover:after {
  z-index: -10;
  animation: fill 1s forwards;
  -webkit-animation: fill 1s forwards;
  -moz-animation: fill 1s forwards;
  opacity: 1;
}
@keyframes fill {
  0% {
    width: 0%;
    height: 1px;
  }
  50% {
    width: 100%;
    height: 1px;
  }
  100% {
    width: 100%;
    height: 100%;
    background:rgb(255,62,0);
  }
}
</style>

<nav class="fill">
	<ul>
		<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">Home</a></li>
		<li><a aria-current="{segment === 'about' ? 'page' : undefined}" href="about">About</a></li>

		<!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		     the blog data when we hover over the link or tap it on a touchscreen -->
		<li><a rel=prefetch aria-current="{segment === 'blog' ? 'page' : undefined}" href="blog">Blog</a></li>
	</ul>
</nav>
