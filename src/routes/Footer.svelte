<script>
  import svelteLogo from "$lib/images/svelte-logo.svg";
</script>

<footer>
  <div class="wrapper">
    <h2 class="link">KMMX</h2>
    <div>
      <span class="link">Bio</span> |
      <span class="link">Archive</span>
      | <span class="link">Ref</span> |
      <span class="link">About me</span>
    </div>
    <div class="footer-content">
      <p class="owner">Kimmix ©2023</p>
      <p>Create using Svelte! <img src={svelteLogo} alt="Svelte" /></p>
      <!-- <p class="block-hover" onclick="switchTheme()">switch theme</p> -->
    </div>
  </div>
  <div class="deco-container">
    <div class="deco1" />
    <div class="diagonal-stripes deco2" />
  </div>
</footer>

<style>
  footer {
    display: flex;
    flex-direction: column;
    gap: 10px;
    min-height: 500px;
    height: 100%;
    background-color: var(--black-color);
    background: linear-gradient(
      0deg,
      var(--black-color) 0%,
      var(--black-color) 60%,
      var(--black2-color) 100%
    );
  }

  img {
    width: 1em;
    height: auto;
  }

  .wrapper {
    z-index: 1;
    flex-direction: column;
    justify-content: end;
    display: flex;
    flex: 1;
    margin-left: 5%;
    gap: 7px;
  }

  .wrapper h2 {
    font-size: 70px;
    line-height: 58px;
  }

  .link {
    transition: color 200ms ease-in;
  }

  .link:hover {
    color: var(--acc2-color);
  }

  .footer-content {
    margin-top: 1.5rem;
    font-weight: 400;
  }

  .footer-content .owner {
    font-weight: 500;
  }

  .deco-container {
    width: 100%;
  }

  .deco-container .deco1 {
    width: 40%;
    height: 0;
    border-style: solid;
    border-width: 30px 30px 0 0;
    border-color: var(--acc2b-color) transparent transparent transparent;
    position: absolute;
    left: 0;
    z-index: 1;
  }

  .deco-container .deco2 {
    width: 100%;
    height: 30px;
    position: absolute;
    left: 0;
  }
</style>
