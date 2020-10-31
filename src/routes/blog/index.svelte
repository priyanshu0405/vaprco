
<svelte:head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</svelte:head>
<style type="text/scss">
  
  .text {
    font: {
      size: calc(2.5vw + 2.5vh);
      family: "Open sans", sans-serif;
      weight: 700;
    }
    margin-left: auto;
    text-transform: uppercase;
		text-align: center;
    position: relative;
    top: 10%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    letter-spacing: 4px;
    white-space: nowrap;

    @media only screen and (max-width: 200px) {
      .text {
        font-size: 1em;
      }
    }
  }

  *{
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: inherit;
}

.column {
  float: left;
  margin-bottom: 5px;
  padding: 0 30px;
}

@media screen and (max-width: 650px) {
  .column {
    width: 100%;
    display:block;
  }
}



.container{
  user-select: none;
  margin: 25px auto;
  background: #231e39;
  max-width:340px;
  min-width:320px;
  color: #b3b8cd;
  border-radius: 5px;
  text-align: center;
  box-shadow: 0 10px 20px -10px rgba(0,0,0,.75);
}
.container::after, .row::after {
  content: "";
  clear: both;
  display: table;
}

.cover-photo{
  background: url(https://images.unsplash.com/photo-1540228232483-1b64a7024923?ixlib=rb-1.2.1&auto=format&fit=crop&w=967&q=80);
  height: 160px;
  width: 100%;
  border-radius: 5px 5px 0 0;
}
.profile{
  height: 100px;
  width: 100px;
  border-radius: 40%;
  margin: 93px 0 0 -175px;
  border: 1px solid #1f1a32;
  padding: 7px;
  background: #292343;
  position:relative;
  
}
.profile:hover{
  -ms-transform: scale(1.5); /* IE 9 */
  -webkit-transform: scale(1.5); /* Safari 3-8 */
  transform: scale(1.5); 
}
.profile-name{
  font-size: 25px;
  font-weight: bold;
  margin: 27px 0 0 120px;
}
.about{
  margin-top: 20px;
  line-height: 21px;
}
.container i{
  padding-left: 20px;
  font-size: 20px;
  margin-bottom: 20px;
  cursor: pointer;
  transition: .5s;
}
i:hover{
  color: #03bfbc;
  opacity: 1;
}
</style>
<div class="text" data-text="our team">our team</div>
<div class="row">
  <div class="column">
    
      <div class="container">
        <div class="cover-photo">
          <img src="https://images.unsplash.com/photo-1565464027194-7957a2295fb7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt=" " class="profile">
        </div>
        <div class="profile-name">Name</div>
        <p class="about">About</p>
        <div>
          <i href="https://github.com/" class="fa fa-align-center fa-github"></i>
          <i href="https://www.linkedin.com/" class="fa fa-linkedin"></i>
          <i href="https://www.instagram.com/" class="fa fa-instagram"></i>
          <i href="https://twitter.com/" class="fa fa-twitter"></i>
          <i href="https://www.facebook.com/" class="fa fa-facebook"></i>
    
        </div>
      </div>
    
  </div>

  <div class="column">
    
      <div class="container">
        <div class="cover-photo">
          <img src="https://images.unsplash.com/photo-1565464027194-7957a2295fb7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt=" " class="profile">
        </div>
        <div class="profile-name">Name</div>
        <p class="about">About</p>
        <div>
          <i href="https://github.com/" class="fa fa-align-center fa-github"></i>
          <i href="https://www.linkedin.com/" class="fa fa-linkedin"></i>
          <i href="https://www.instagram.com/" class="fa fa-instagram"></i>
          <i href="https://twitter.com/" class="fa fa-twitter"></i>
          <i href="https://www.facebook.com/" class="fa fa-facebook"></i>
    
        </div>
      </div>
    
  </div>
  
  <div class="column">
    
      <div class="container">
        <div class="cover-photo">
          <img src="https://images.unsplash.com/photo-1565464027194-7957a2295fb7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt=" " class="profile">
        </div>
        <div class="profile-name">Name</div>
        <p class="about">About</p>
        <div>
          <i href="https://github.com/" class="fa fa-align-center fa-github"></i>
          <i href="https://www.linkedin.com/" class="fa fa-linkedin"></i>
          <i href="https://www.instagram.com/" class="fa fa-instagram"></i>
          <i href="https://twitter.com/" class="fa fa-twitter"></i>
          <i href="https://www.facebook.com/" class="fa fa-facebook"></i>
    
        </div>
      </div>
    
  </div>

  <div class="column">
    
      <div class="container">
        <div class="cover-photo">
          <img src="https://images.unsplash.com/photo-1565464027194-7957a2295fb7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt=" " class="profile">
        </div>
        <div class="profile-name">Name</div>
        <p class="about">About</p>
        <div>
          <i href="https://github.com/" class="fa fa-align-center fa-github"></i>
          <i href="https://www.linkedin.com/" class="fa fa-linkedin"></i>
          <i href="https://www.instagram.com/" class="fa fa-instagram"></i>
          <i href="https://twitter.com/" class="fa fa-twitter"></i>
          <i href="https://www.facebook.com/" class="fa fa-facebook"></i>
    
        </div>
      </div>
    
  </div>

  <div class="column">
    
    <div class="container">
      <div class="cover-photo">
        <img src="https://images.unsplash.com/photo-1565464027194-7957a2295fb7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt=" " class="profile">
      </div>
      <div class="profile-name">Name</div>
      <p class="about">About</p>
      <div>
        <i href="https://github.com/" class="fa fa-align-center fa-github"></i>
        <i href="https://www.linkedin.com/" class="fa fa-linkedin"></i>
        <i href="https://www.instagram.com/" class="fa fa-instagram"></i>
        <i href="https://twitter.com/" class="fa fa-twitter"></i>
        <i href="https://www.facebook.com/" class="fa fa-facebook"></i>
  
      </div>
    </div>
  
  </div>

  <div class="column">
    
    <div class="container">
      <div class="cover-photo">
        <img src="https://images.unsplash.com/photo-1565464027194-7957a2295fb7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=80" alt=" " class="profile">
      </div>
      <div class="profile-name">Name</div>
      <p class="about">About</p>
      <div>
        <i href="https://github.com/" class="fa fa-align-center fa-github"></i>
        <i href="https://www.linkedin.com/" class="fa fa-linkedin"></i>
        <i href="https://www.instagram.com/" class="fa fa-instagram"></i>
        <i href="https://twitter.com/" class="fa fa-twitter"></i>
        <i href="https://www.facebook.com/" class="fa fa-facebook"></i>
  
      </div>
    </div>
  
</div>

</div>

