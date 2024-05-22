<!-- <template>
    <div>
      <button @click="viewAsBlocks = true">Ver como bloques</button>
      <button @click="viewAsBlocks = false">Ver como lista</button>
  
      <div v-if="viewAsBlocks" class="block-view">
        <div v-for="post in posts" :key="post.id" class="post-block">
          <h3>{{ post.title }}</h3>
          <p>{{ post.summary }}</p>
        </div>
      </div>
  
      <ul v-else class="list-view">
        <li v-for="post in posts" :key="post.id" class="post-list">
          <h3>{{ post.title }}</h3>
          <p>{{ post.summary }}</p>
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        viewAsBlocks: true,
        posts: [
          { id: 1, title: 'Publicación 1', summary: 'Resumen de la publicación 1' },
          { id: 2, title: 'Publicación 2', summary: 'Resumen de la publicación 2' },
          { id: 3, title: 'Publicación 3', summary: 'Resumen de la publicación 3' },
          { id: 4, title: 'Publicación 4', summary: 'Resumen de la publicación 4' },
          { id: 5, title: 'Publicación 5', summary: 'Resumen de la publicación 5' },
          { id: 6, title: 'Publicación 6', summary: 'Resumen de la publicación 6' },
        ]
      };
    }
  }
  </script>
  <style scoped>
  .block-view {
    display: flex;
    flex-wrap: wrap;
  }
  
  .post-block {
    width: 30%;
    margin: 1%;
    padding: 10px;
    border: 1px solid #ccc;
    box-shadow: 2px 2px 6px #aaa;
  }
  
  .list-view {
    list-style-type: none;
    padding: 0;
  }
  
  .post-list {
    padding: 10px;
    border-bottom: 1px solid #ccc;
  }
  </style> -->