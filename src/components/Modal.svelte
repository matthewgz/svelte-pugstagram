<style>
  .Modal {
    position: relative;
  }
  .Modal-overlay {
    align-items: center;
    background-color: rgba(0, 0, 0, 0.7);
    bottom: 0;
    cursor: pointer;
    display: flex;
    justify-content: center;
    left: 0;
    position: fixed;
    right: 0;
    top: 0;
    z-index: 8;
  }
</style>

<div class="Modal">
  <div class="Modal-overlay" >
    <slot />
  </div>
</div>
