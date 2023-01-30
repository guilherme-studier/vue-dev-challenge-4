<template>
  <div class="cook">
    <span class="material-symbols-outlined icon-restaurant" :class="icon">{{ icon }}</span>
    <div class="cooking-time">
      <h3 class="title">{{ title }}</h3>
      <h3 class="subtitle" :class="icon">{{ subtitle }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Cook',
  props: {
    icon: {
      type: String,
      default: null
    },
    title: {
      type: String,
      default: null
    },
    subtitle: {
      type: String,
      default: null
    }
  }
}
</script>

<style scoped>
  .cook {
    display: flex;
  }

  .cook .cooking-time {
    text-align: initial;
    margin-left: 14.03px;
  }

  .cook span {}

  .cook .title {
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 10px;
    line-height: 12px;
    color: var(--gray-600);
    text-transform: uppercase;
  }

  .cook .subtitle {
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 17px;
  }


  .schedule {
    color: var(--gray-800);
  }

  .restaurant_menu {
    color: var(--orange-500)
  } 

  @media (max-width: 700px) {
    .cook .cooking-time {
      margin-left: 5.42px;
    }
  }
</style>