<!-- home -->

<%- include('./partials/header.ejs') -%>

  <h1>Home</h1>
  <p><%= startingContent %></p>

  <% for (let i=0; i<posts.length; i++) { %>
    <h1><%= posts[i].title %></h1>
    <p><%= posts[i].content %></p>
  <% } %>

  <% posts.forEach((post) => { %>
    <h1><%= post.title %></h1>
    <p><%= post.content %></p>
  <% }) %>
  

<%- include('./partials/footer.ejs') -%>