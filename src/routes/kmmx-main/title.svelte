<section class="title page">
  <div class="logo-bg">
    <svg
      id="animate-onscroll"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 357.44 313.09"
    >
      <path
        class="stroke"
        d="M9.17 298.17 203.07 8.23 203.07 298.17 145.17 206.27 9.17 298.17z"
      />
      <path
        class="stroke"
        d="M223.29 301.84 223.29 133.67 347.81 304.14 280.72 262.33 223.29 301.84z"
      />
    </svg>
  </div>
  <div class="logo-wrapper">
    <svg
      id="logoFill"
      xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink"
      viewBox="0 0 338.64 295.91"
    >
      <defs>
        <style>
          .logoFill1 {
            fill: url(#SVGID_1);
          }

          .logoFill2 {
            fill: url(#SVGID_2);
          }
        </style>
        <radialGradient
          id="SVGID_1"
          cx="198"
          cy="290"
          r="281.0872"
          gradientUnits="userSpaceOnUse"
        >
          <stop offset="0" style="stop-color:#F9826C" />
          <stop offset="1" style="stop-color:#FF446C" />
        </radialGradient>
        <polygon class="st0" points="0,289.9 193.9,0 193.9,289.9 136,198 " />
        <radialGradient
          id="SVGID_2"
          cx="211"
          cy="295"
          r="166.0753"
          gradientUnits="userSpaceOnUse"
        >
          <stop offset="0" style="stop-color:#F9826C" />
          <stop offset="1" style="stop-color:#FF446C" />
        </radialGradient>
      </defs>
      <polygon
        class="logoFill1"
        points="0 289.94 193.9 0 193.9 289.94 136 198.04 0 289.94"
      />
      <polygon
        class="logoFill2"
        points="214.12 293.61 214.12 125.44 338.64 295.91 271.55 254.1 214.12 293.61"
      />
    </svg>
  </div>
  <div class="wrapper">
    <div class="header-wrapper">
      <div class="swipe">
        <span class="block1" id="animate-onscroll" />
        <div class="title" id="animate-onscroll">KMMX</div>
      </div>
      <div class="swipe">
        <span class="block2" id="animate-onscroll" />
        <div class="subtitle" id="animate-onscroll">
          <h2>
            <span class="V">V</span><span class="H">H</span><span class="E"
              >E</span
            >OS 2.1.0
          </h2>
        </div>
      </div>
    </div>
  </div>
  <span class="scrollline" />
</section>

<style>
  section {
    width: 100%;
    min-height: 100vh;
    display: flex;
    position: relative;
  }

  /* Logo */

  .logo-wrapper {
    position: absolute;
    right: 0;
    height: 100%;
    width: clamp(17rem, 39vw, 34rem);
    overflow-x: hidden;
  }

  .title svg .stroke {
    fill: none;
    stroke: var(--acc2b-color);
    stroke-width: 4px;
    stroke-dasharray: 912;
    stroke-dashoffset: 912;
    animation: stroke-anim 3.5s ease-out forwards 500ms;
  }

  @keyframes stroke-anim {
    to {
      stroke-dashoffset: 0;
    }
  }

  .title svg#logoFill {
    margin-top: 10vw;
    animation: hover 5s infinite alternate 8.5s, fadeIn 2s 8.5s,
      show 1s infinite 9.5s;
    opacity: 0;
  }

  @keyframes show {
    0% {
      opacity: 1;
    }

    100% {
      opacity: 1;
    }
  }

  @keyframes hide {
    0% {
      opacity: 0;
    }

    100% {
      opacity: 0;
    }
  }

  @keyframes hover {
    0% {
      transform: translateY(0);
    }

    40% {
      transform: translateY(2%);
    }

    60% {
      transform: translateY(1%);
    }

    100% {
      transform: translateY(0);
    }
  }

  /* Title */

  section.title {
    justify-content: center;
    overflow: visible;
  }

  section.title > .logo-bg {
    position: absolute;
    right: 0;
    bottom: 0;
    width: clamp(600px, 60vw, 900px);
    height: 80%;
  }

  section.title > .wrapper {
    width: 100%;
    display: flex;
    max-width: 1500px;
    justify-content: space-between;
    margin: 3em 10px;
  }

  .header-wrapper {
    min-width: clamp(18rem, 80vw, 36em);
    position: relative;
    display: flex;
    justify-content: center;
    flex-direction: column;
  }

  .swipe {
    width: 100%;
    position: relative;
    display: flex;
    align-items: center;
  }

  .swipe .title {
    width: 100%;
    font-size: clamp(3rem, 18vw, 11em);
    letter-spacing: 10px;
    text-align: center;
    color: var(--white-color);
    opacity: 0;
    animation: fadeIn 2s forwards 7.6s, fadeIn 3.5s forwards 2.4s;
  }

  .swipe .subtitle {
    width: 100%;
    opacity: 0;
    margin-right: 2rem;
    cursor: pointer;
    animation: fadeIn 2s forwards 2.6s;
  }

  .swipe .subtitle h2 {
    display: flex;
    justify-content: flex-end;
    padding: 0;
    margin: 0;
    font-size: clamp(0.9rem, 4vw, 1.7em);
    letter-spacing: 5px;
    text-align: right;
    color: var(--white2-color);
  }

  .swipe span.block1 {
    z-index: 2;
    width: 0%;
    height: 100%;
    position: absolute;
    display: flex;
    background-color: var(--acc1-color);
    animation: mainBlock 1.8s cubic-bezier(0.74, 0.06, 0.4, 0.92) forwards 1.3s,
      mainBlock 2s cubic-bezier(0.74, 0.06, 0.4, 0.92) forwards 5s;
  }

  .swipe span.block2 {
    z-index: 2;
    width: 0%;
    height: 100%;
    position: absolute;
    display: flex;
    background-color: var(--acc2-color);
    animation: mainBlock 2s cubic-bezier(0.74, 0.06, 0.4, 0.92) forwards 1.1s;
  }

  span.scrollline {
    height: 0;
    width: 14px;
    background: repeating-linear-gradient(
      to top,
      var(--white-color) 0,
      var(--white-color) 5px,
      transparent 5px,
      transparent 12px
    );
    position: absolute;
    left: 30px;
    bottom: 0;
    animation: run 3s infinite 10s;
  }

  @keyframes run {
    0% {
      height: 300px;
      transform: translateY(-50%) scaleY(0);
    }

    60% {
      transform: translateY(-20%) scaleY(1);
    }

    80% {
      transform: translateY(0) scaleY(0);
    }

    100% {
      transform: translateY(-50%) scaleY(0);
    }
  }

  @keyframes mainBlock {
    0% {
      width: 0%;
      left: 0;
    }

    50% {
      width: 100%;
      left: 0;
    }

    100% {
      width: 0;
      left: 100%;
    }
  }

  @keyframes secBlock {
    0% {
      width: 0%;
      left: 0;
    }

    50% {
      width: 100%;
      left: 0;
    }

    100% {
      width: 0;
      left: 100%;
    }
  }

  @keyframes fadeIn {
    0% {
      opacity: 0;
    }

    100% {
      opacity: 1;
    }
  }

  /* V.H.E. */
  .subtitle > h2 span {
    display: flex;
    overflow: hidden;
  }

  .V:after {
    content: ".";
  }

  .V:hover,
  .V:active {
    color: var(--acc2-color);
  }

  .V:hover:after,
  .V:active:after {
    content: "ery";
    animation: reveal 700ms ease-out forwards;
  }

  .H:after {
    content: ".";
  }

  .H:hover,
  .H:active {
    color: var(--acc2-color);
  }

  .H:hover:after,
  .H:active:after {
    content: "igh";
    animation: reveal 700ms ease-out forwards;
  }

  .E:after {
    content: ".";
  }

  .E:hover,
  .E:active {
    color: var(--acc2-color);
  }

  .E:hover:after,
  .E:active:after {
    content: "fficiency";
    animation: reveal 450ms ease-out forwards;
  }

  @keyframes reveal {
    from {
      max-width: 1rem;
    }

    to {
      max-width: 200px;
    }
  }

  @media screen and (max-width: 768px) {
    .header-wrapper {
      margin-bottom: 30vh;
    }

    svg#logoFill {
      width: 100%;
      margin-left: 3em;
      margin-top: 55vh;
    }

    section.title {
      justify-content: center;
    }
  }

  @media screen and (min-width: 1400px) {
    .header-wrapper {
      padding-left: 15%;
    }
  }
</style>
