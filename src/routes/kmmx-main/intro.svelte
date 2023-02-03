<div class="intro">
  <div class="text-wrapper">
    <div class="text-0 text">Initializing completed</div>
  </div>
  <div class="text-wrapper">
    <div class="text-1 text outline">...system initializing...</div>
    <div class="text-2 text">...system initializing...</div>
    <div class="text-3 text outline">...system initializing...</div>
    <div class="text-4 text outline">...system initializing...</div>
    <div class="text-5 text">...system initializing...</div>
    <div class="text-6 text">...system initializing...</div>
    <div class="text-7 text">...system initializing...</div>
    <div class="text-8 text outline">...system initializing...</div>
    <div class="text-9 text">...system initializing...</div>
    <div class="text-10 text outline">...system initializing...</div>
  </div>
  <div class="text-wrapper">
    <div class="text-error text">
      system initializing system initializing system initializing
    </div>
  </div>
</div>

<style>
  div.intro {
    position: fixed;
    width: 100%;
    height: 100vh;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 999;
    background-color: var(--black2-color);
    -webkit-user-select: none;
    -khtml-user-select: none;
    -moz-user-select: none;
    -o-user-select: none;
    user-select: none;
    animation: delete-out-container 1s linear forwards 5.5s;
  }

  .text-wrapper {
    position: absolute;
    display: flex;
    flex-direction: column;
    width: 100%;
    height: 100vh;
  }

  .text {
    margin: auto;
    font-size: clamp(1.7rem, -0.875rem + 8.333vw, 5rem);
    color: var(--white-color);
  }

  .text-0 {
    font-size: clamp(1rem, 100px, 3.5rem);
    animation: slide-out 1.5s linear 3.5s;
    opacity: 0;
  }

  .text-1 {
    animation: blink 0.8s linear 0.9s, blink 0.5s linear 2s;
    opacity: 0;
  }

  .text-2 {
    animation: blink 0.8s linear 0.8s, blink 0.6s linear 2s;
    opacity: 0;
  }

  .text-3 {
    animation: blink 0.8s linear 0.7s, blink 0.65s linear 2s;
    opacity: 0;
  }

  .text-4 {
    animation: blink 0.8s linear 0.9s, blink 0.7s linear 2s;
    opacity: 0;
  }

  .text-5 {
    animation: blink 0.8s linear 0.7s, blink 0.75s linear 2s;
    opacity: 0;
  }

  .text-6 {
    animation: blink 0.8s linear 0.8s, blink 0.75s linear 2s;
    opacity: 0;
  }

  .text-7 {
    animation: blink 0.8s linear 0.9s, blink 0.7s linear 2s;
    opacity: 0;
  }

  .text-8 {
    animation: blink 0.8s linear 0.7s, blink 0.65s linear 2s;
    opacity: 0;
  }

  .text-9 {
    animation: blink 0.8s linear 0.6s, blink 0.6s linear 2s;
    opacity: 0;
  }

  .text-10 {
    animation: blink 0.8s linear 0.8s, blink 0.5s linear 2s;
    opacity: 0;
  }

  .text-error {
    font-size: clamp(4rem, 400px, 20rem);
    color: red;
    overflow: hidden;
    text-overflow: clip;
    width: 100%;
    height: 100vh;
    animation: blink 0.8s linear 2.8s;
    opacity: 0;
  }

  @keyframes blink {
    0% {
      opacity: 0;
    }

    1% {
      opacity: 100%;
    }

    99% {
      opacity: 100%;
    }

    100% {
      opacity: 0;
    }
  }

  @keyframes slide-out {
    0% {
      opacity: 0;
    }

    1% {
      opacity: 100%;
    }

    19% {
      opacity: 100%;
    }

    20% {
      opacity: 0;
    }

    69% {
      opacity: 100%;
    }

    70% {
      opacity: 100%;
    }

    100% {
      opacity: 0;
    }
  }

  @keyframes delete-out-container {
    99% {
      height: initial;
    }

    100% {
      opacity: 0;
      height: 0;
      display: none;
    }
  }
</style>
