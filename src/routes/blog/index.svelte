<style type="text/scss">
  :global(body) {
    background-color: black;
  }
  .glitch {
    font: {
      size: calc(4vw + 4vh);
      family: "Open sans", sans-serif;
      weight: 700;
    }
    text-transform: uppercase;
		text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    letter-spacing: 4px;
    white-space: nowrap;

    @media only screen and (max-width: 200px) {
      .glitch {
        font-size: 1em;
      }
    }
  }
</style>

<div class="glitch" data-glitch="our team">our team</div>
