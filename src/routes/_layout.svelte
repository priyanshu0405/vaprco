<script>

	import Nav from '../components/Nav.svelte';
	import Icon from 'svelte-awesome/components/Icon.svelte';
import {twitter, facebook, github, linkedin, instagram } 
from 'svelte-awesome/icons';
	export let segment;
</script>

<style>
	main {
		position: relative;
		max-width: 56em;
		padding: 5em;
		margin: 0 auto;
		box-sizing: border-box;
	}


.footer-icons{	
  font-size:2em;
  width:100%;
  position:fixed;
  bottom:0px;
  /*width:auto;*/
}

ul{
  display: flex;
  flex-direction:row;
  justify-content:center;
  /*align-content:space-between;*/

}

ul li {
  list-style: none;
  padding:0.5em;
}

ul li a{
  opacity:0.5;
  color:silver;
  line-height: 90px;
  text-align:center;
  margin:auto;
  padding:0.2em;
  display: inline-block;
  overflow: hidden;
}

a:hover{
  color:white;
  opacity:1;
}


</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>

  <footer class="footer">
	<div class="col-sm-12 text-center">
		<div class="footer-icons">
      <ul>
      <li><a href="https://github.com/"><Icon scale="3" class="fa fa-align-center fa-github" data="{github}" /></a></li>
      <li><a href="https://www.linkedin.com/"><Icon scale="3" class="fa fa-linkedin" data="{linkedin}" /></a></li>
      <li><a href="https://www.instagram.com/"><Icon scale="3" class="fa fa-instagram" data="{instagram}" /></a></li>
      <li><a href="https://twitter.com/"><Icon scale="3" class="fa fa-twitter" data="{twitter}" /></a></li>
      <li><a href="https://www.facebook.com/"><Icon scale="3" class="fa fa-facebook" data="{facebook}" /></a></li>
      
      </ul>
      
	</div>
</div>
    </footer>