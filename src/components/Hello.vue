<template>
<div>

  	<!-- Page Contents -->
  	<div class="pusher">
  	  <div class="ui inverted vertical masthead center aligned segment">

        <div class="ui text container">
            <h1 class="ui inverted header">
                Music Cloud
            </h1>
            <h3>Discover, stream, and share a constantly expanding mix of music from emerging and major artists around the world.</h3>
            <div id="search-bar" class="ui huge inverted transparent icon input">
                <input type="text" placeholder="Search for artists, bands, tracks, podcasts..">
                <i class="search icon"></i>
            </div>
        </div>

  	  </div>

  	  <div class="ui vertical stripe segment">
  		<div class="ui middle aligned stackable grid container">
  		  <div class="row">
  			<div class="seven wide column">
  			  <h3 class="ui header">Connect on MusicCloud</h3>
  			  <p>Get on SoundCloud to connect with fans, share your sounds, and grow your audience.</p>
  			  <h3 class="ui header">We Make Trends</h3>
  			  <p>Hear what’s trending for free in the MusicCloud community.</p>
  			</div>
  			<div class="seven wide right floated column">
  			  <!-- <img src="/static/images/mbls.png" class="ui large bordered rounded image"> -->
          <div class="ui small images">
            <img src="/static/images/song1.png">
            <img src="/static/images/song2.png">
            <img src="/static/images/song3.png">
            <img src="/static/images/song4.png">
            <img src="/static/images/song5.png">
            <img src="/static/images/song6.png">
          </div>
  			</div>
  		  </div>
  		  <div class="row">
  			<div class="center aligned column">
  			  <a class="ui large basic secondary button">Explore Top Charts</a>
  			</div>
  		  </div>
  		</div>
  	  </div>


  	  <div class="ui vertical stripe quote segment">
  		<div class="ui equal width stackable grid">
  		  <div class="centered row">
            <div class="one wide column"></div>
  			<div class="six wide center aligned column">
  			  <h3>Never stop listening</h3>
  			  <p>MusicCloud is available on Web, Mobile, Sonos, Google Chromecast, and Microsoft Xbox One</p>
              <p>Get it on</p>
              <div class="ui big basic buttons">
                <button class="ui  button"><i class="apple icon"></i>App Store</button>
                <div class="or"></div>
                <button class="ui button"><i class="play icon"></i>Google Play</button>
              </div>
  			</div>
            <div class="two wide column"></div>
  			<div class="seven wide center aligned column">
  			  <p>
  				<img class="ui large image" src="/static/images/mbls.png">
  			  </p>
  			</div>
  		  </div>
  		</div>
  	  </div>

  	  <div class="ui vertical stripe center aligned segment">
  		<div class="ui text container">
  		  <h3 class="ui header">Calling all creators</h3>
  		  <p>Get on SoundCloud to connect with fans, share your sounds, and grow your audience. What are you waiting for?</p>
  		  <a class="ui secondary basic large button">Find out more</a>

  		  <h3 class="ui header">Thanks for listening. Now join in.</h3>
  		  <p>Save tracks, follow artists and build playlists. All for free.</p>
  		  <a class="ui secondary large button" @click="openSignupModal">Create Account</a>
  		</div>
  	  </div>

  	</div>

</div>
</template>

<script>

export default {
  name: 'hello',
  data () {
    return {
    }
  },
  methods: {
    openSignupModal () {
      $('#signup').modal('show');
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  #search-bar{
    width: 500px;
    margin-top: 20px;
  }

  .hidden.menu {
    display: none;
  }

  .masthead.segment {
    min-height: 700px;
    padding: 1em 0em;
  }
  .masthead .logo.item img {
    margin-right: 1em;
  }
  .masthead .ui.menu .ui.button {
    margin-left: 0.5em;
  }
  .masthead h1.ui.header {
    margin-top: 3em;
    margin-bottom: 0em;
    font-size: 4em;
    font-weight: normal;
  }
  .masthead h2 {
    font-size: 1.7em;
    font-weight: normal;
  }

  .ui.vertical.stripe {
    padding: 8em 0em;
  }
  .ui.vertical.stripe h3 {
    font-size: 2em;
  }
  .ui.vertical.stripe .button + h3,
  .ui.vertical.stripe p + h3 {
    margin-top: 3em;
  }
  .ui.vertical.stripe .floated.image {
    clear: both;
  }
  .ui.vertical.stripe p {
    font-size: 1.33em;
  }
  .ui.vertical.stripe .horizontal.divider {
    margin: 3em 0em;
  }

  .quote.stripe.segment {
    padding: 0em;
  }
  .quote.stripe.segment .grid .column {
    padding-top: 5em;
    padding-bottom: 5em;
  }

  .secondary.pointing.menu .toc.item {
    display: none;
  }

  @media only screen and (max-width: 700px) {

    #search-bar{
      width: 300px;
      margin-top: 20px;
    }

    .ui.fixed.menu {
      display: none !important;
    }
    .secondary.pointing.menu .item,
    .secondary.pointing.menu .menu {
      display: none;
    }
    .secondary.pointing.menu .toc.item {
      display: block;
    }
    .masthead.segment {
      min-height: 350px;
    }
    .masthead h1.ui.header {
      font-size: 2em;
      margin-top: 1.5em;
    }
    .masthead h2 {
      margin-top: 0.5em;
      font-size: 1.5em;
    }
  }

</style>
