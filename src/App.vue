<script setup>

</script>

<template>
  <main>
  <h1 class="title">My Vue Grocery List ✎</h1>
  <form class="newGroceryForm">
        <input id="newGrocery" 
        autocomplete="off"
        type="text" 
        placeholder="Add an item to your list" />
        <button id="addBtn" type="submit">Add</button>
    </form>

    <ul>
      <li>Chips</li>
    </ul>
</main>
</template>

<style lang="postcss" scoped>
main {

  @apply flex flex-col justify-center items-center mt-8 gap-8;

.title {
  
  @apply m-2 text-6xl font-light tracking-wider text-background;
  }

  form {
    @apply  flex focus-within:ring-8 focus-within:ring-background focus-within:rounded-lg;
    
    input {
      @apply bg-white text-comment p-2 w-80 text-2xl rounded-l-md outline-none;
    }
    button {
      @apply bg-background text-yellowish p-2 text-2xl font-bold rounded-r-md;

      &:hover {
        @apply bg-purplish;
      }
    }
  }

  ul {
    @apply flex flex-col items-center justify-center rounded-lg bg-comment;
    li {
      @apply bg-white text-background m-2 p-2 w-96 text-center;
      &:hover {
        @apply bg-yellowish font-bold cursor-pointer;
      }
    }
  }
}

</style>
