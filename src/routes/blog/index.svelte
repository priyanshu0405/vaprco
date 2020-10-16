<style type="text/scss">
  .text {
    font: {
      size: calc(2.5vw + 2.5vh);
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
      .text {
        font-size: 1em;
      }
    }
  }
</style>

<div class="text" data-text="our team">our team</div>
