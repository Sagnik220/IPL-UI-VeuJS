<template>
  <nav>
    <div class="menu-item"><a href="#">Home</a></div>
    <Dropdown title="Teams" :items="Teams" />
    <div class="menu-item"><a href="#">Points Table</a></div>
    <div class="menu-item"><a href="#">More</a></div>
  </nav>
</template>

<script>
import Dropdown from './Dropdown';
export default {
  name: 'navbar',
  components: {
    Dropdown
  },
  data () {
    return {
      Teams: [
        {
          title: 'CSK',
          link:'#'
        },
        {
          title: 'DC',
          link: '#'
        },
        {
            title:'KKR',
            link: '#'
        },
        {
          title: 'KXIP',
          link: '#'
        },
        {
          title: 'MI',
          link: '#'
        },
        {
          title: 'SRH',
          link: '#'
        },
        {
          title: 'RCB',
          link: '#'
        },
        {
          title: 'RR',
          link: '#'
        },
      
      ]
    }
  }
}
</script>

<style>
nav {
  display: flex;
  align-items: center;
  justify-content: center;
}
nav .menu-item {
  color: #FFF;
  padding: 10px 20px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: flex;
  transition: 0.4s;
}
nav .menu-item.active,
nav .menu-item:hover {
  background-color: #444;
  border-bottom-color: #FF5858;
}
nav .menu-item a {
  color: inherit;
  text-decoration: none;
}
</style>