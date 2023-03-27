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
    background-color: #333;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    padding: 0.5rem 1rem;
}

.logo {
    font-weight: bold;
    font-size:2.5rem;
    color: red;
    animation: shake 0.5s infinite;
}
@keyframes shake {
    0% { transform: translateX(0); }
    25% { transform: translateX(-5px) rotate(0.5deg); }
    50% { transform: translateX(0) rotate(0deg); }
    75% { transform: translateX(5px) rotate(-0.5deg); }
    100% { transform: translateX(0); }
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
marquee {
    color: red;
    background-color: #333;
    padding: 0.5rem;
    white-space: nowrap;
    overflow: hidden;
    animation: marquee 10s linear infinite;
}
</style>
