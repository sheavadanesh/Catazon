# Artazon

<a href='http://artazon.herokuapp.com/'>Live Site</a>

<h3>Table of Contents</h3>

<ul>
  <li>Background</li>
  <li>Technologies</li>
  <li>Features
    <ul>
      <li>User Authentication</li>
      <li>Items Index</li>
      <li>Item Show</li>
    </ul>
  </li>
</ul>

<h3>Background</h3>

<p>
  Artazon is a full stack web application used to buy/sell famous artworks, inspired by the website Amazon. This application allows users to create an account and sign in, storing their inputted data in the PostgreSQL database. There is also an option for users to continue into the application using a guest login feature. This way the user does not need to create an account to browse through different products and get the full customer experience. On the items index page, users are able to interact with individual items, clicking into the item show page to view details and potentially purchase the item.

  This site was built on a Ruby on Rails framework for the backend with Active Record to avoid N+1 queries. The database utilized to store user/product data was PostgreSQL, along with Amazon AWS S3 which was used to store product images. React and Redux with Node.js were the technologies used for frontend frameworks in order to create a dynamic, single-page web application, allowing for a smooth navigation throughout the website. 
</p>

<h3>Technologies</h3>

<ul>
    <li>Ruby (v 2.5.1)</li>
    <li>Rails (v 5.2.4.3)</li>
    <li>React.js</li>
    <li>Redux.js</li>
    <li>Node.js</li>
    <li>PostgreSQL</li>
    <li>Webpack</li>
    <li>Amazon AWS S3</li>
</ul>

<h3>Features</h3>

<h4>User Authentication</h4>

<ul>
    <li>Users can sign up and create an account on Artazon, storing their information to be able to logout and log back in to view their personal account.</li>
    <li>The sign-in and signup forms are separate components which were made using React/Redux and CSS for styling purposes. These forms can be accessed through a dropdown menu from the navigation bar or by clicking on explicit links on the home page. </li>
    <li>For users who do not want to create their own account but still want to explore the full features of the website, a demo login feature is available that serves as a guest login.</li>
</ul>

<h4>Items Index</h4>

<ul>
    <li>All items are rendered when accessing the home page (which can be accessed by entering the website's URL or clicking on any Artazon logo) or first logging into a user's account.</li>
    <li>Users can go directly to an item's show page by clicking on either the item's title or image on the list. </li>
</ul>

<h4>Item Show Page</h4>

<ul>
    <li>Users can view each item's information page, which includes a high-res image of the art piece, the artist and year created, style and media type, a short description, and the price to purchase the item. </li>
    <li>On the right-most side of the show page is a component that users will be able to use in order to either add an item to their shopping cart or purchase the item without a cart using the "Buy Now" button.</li>
    <li>Below the item description and image, there is a section where users can rate and review the item if they are signed in with their account.</li>
    <li>Right below the item's title will be an average rating that the item has received so far.</li>
    <li>Each item's image is linked from a bucket created in Amazon AWS S3.</li>
</ul>
