<template>
    <header>
    <div class="logo">MOVIEFLIX
    </div>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
    </header>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
    name: 'Header',
  // Headerコンポーネントのプロパティやメソッドを定義する
}
</script>

<style>
header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #fff;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    padding: 0.5rem 1rem;
}

.logo {
  font-weight: bold;
  font-size: 1.5rem;
}

nav ul {
  display: flex;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

nav li {
  margin-right: 1rem;
}

nav a {
  color: #333;
  text-decoration: none;
}
</style>
