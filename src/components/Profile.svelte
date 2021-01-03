<script>
  export let name;
  export let nickname;
</script>

<style>
  .Profile-content {
    display: flex;
    align-items: center;
  }
  .Profile-avatar img {
    width: 42px;
    height: 42px;
    border-radius: 50%;
  }
  .Profile-info {
    margin: 0 0 0 0.5em;
  }
  .Profile-info h2 {
    font-size: 14px;
    color: black;
    margin: 0;
    padding: 0;
  }
  .Profile-info span {
    font-size: 12px;
    font-weight: normal;
  }
</style>

<div class="Prodile">
  <div class="Profile-content">
    <div class="Profile-avatar">
      <img
        src="https://www.discordianos.com/uploads/monthly_2020_07/fotopelelaperfil.jpg.384d7c7d3bb5f4a52983b5bc0aad212c.jpg"
        alt="Foto de perfil" />
    </div>
    <div class="Profile-info">
      <h2>{nickname}</h2>
      <span>{name}</span>
    </div>
  </div>
</div>
