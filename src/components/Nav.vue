<template>
  <nav>
    <ul>
      <li v-for="item in items">
        <a :href="item.href">{{item.text}}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
let items = [
  {
    text: 'lazylife',
    href: '#'
  }
]
export default {
  name: 'Nav',
  data () {
    return {
      items: items
    }
  }
}
</script>

<style lang="scss" scoped>
nav {
  margin: 0;
  padding: 1rem;
  border-bottom: solid #222 0.4rem;
  ul {
    margin: 0;
    padding: 0;
    list-style-type: none;
    text-align: left;
    li {
      display: inline-block;
      padding: 0 0.8rem;
      vertical-align: middle;
      a {
        outline: none;
        text-decoration: none;
        color: #222;
        font-size: 1.25rem;
      }
      a:hover {
        font-weight: bold;
      }
    }
  }
}
</style>
