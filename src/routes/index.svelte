<style type="text/scss">
  :global(body) {
    background-color: black;
  }
  .glitch {
    font: {
      size: 10em;
      family: "Penna", sans-serif;
      weight: 700;
    }
    text-decoration: none;
    text-transform: uppercase;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    margin: 0;
    color: white;
    letter-spacing: 5px;

    &:before,
    &:after {
      display: block;
      content: attr(data-glitch);
      text-transform: uppercase;
      position: absolute;
      top: 0;
      left: 0;
      height: 100%;
      width: 100%;
      opacity: 0.8;
    }
    &:after {
      color: #f0f;
      z-index: -2;
    }
    &:before {
      color: #0ff;
      z-index: -1;
    }
    &:hover {
      &:before {
        animation: glitch 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94) both 5;
      }
      &:after {
        animation: glitch 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94) reverse both
          5;
      }
    }
  }

  @media only screen and (max-width: 400px) {
    .glitch {
      font-size: 3em;
    }
  }

  @keyframes glitch {
    0% {
      transform: translate(0);
    }
    20% {
      transform: translate(-5px, 5px);
    }
    40% {
      transform: translate(-5px, -5px);
    }
    60% {
      transform: translate(5px, 5px);
    }
    80% {
      transform: translate(5px, -5px);
    }
    to {
      transform: translate(0);
    }
  }
</style>

<div class="glitch" data-glitch="VAPRCO">VAPRCO</div>
