<style>
  .Share {
    background-color: white;
    border-radius: 4px;
    border: 1px solid rgba(219, 219, 219, 1);
    height: 80px;
    margin: 0 0 2em 0;
    padding: 1em;
    width: 300px;
  }
  .Share-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .Share-head h2 {
    font-size: 16px;
  }
  .Share-head i {
    cursor: pointer;
  }
  .Share-content a {
    display: flex;
    align-items: center;
    text-decoration: none;
    color: black;
    font-size: 14px;
    margin: 2em 0 0 0;
  }
  .Share-content i {
    color: #3b5998;
    margin: 0 0.5em 0 0;
    font-size: 20px;
  }
</style>

<div class="Share">
  <div class="Share-head">
    <h2>Compartir</h2>
    <i class="fas fa-times-circle" on:click />
  </div>
  <div class="Share-content">
    <a
      href="https://www.facebook.com/sharer.php?&u=https://svelt-pugstagram.netlify.app/"
      target="_blank">
      <i class="fab fa-facebook-square" />
      Compartir en Facebook
    </a>
  </div>
</div>
