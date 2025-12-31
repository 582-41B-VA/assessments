# Milestone 1: Models

> Due: January 28

Milestone 1 focuses on defining models and setting up views. Here are
the requirements:

- Products have a name, description, image, price, quantity, and
  creation date. You may add additional fields if necessary.

- Products have an `is_available` property that is true when their
  quantity is greater than 0.

- Products belong to a category. Categories have a name and a
  description.

- Products and categories can be added and modified from the built-in
  admin panel.

- On the home page, users can see a list of all products currently
  available. Products are sorted by their creation date, from newest to
  oldest.

- The home page includes a list of categories. Clicking on a category
  brings users to a page where products from that category are listed.
  On the category page, the name and the description of the category is
  shown.

- Clicking on a product brings users to a details page where information
  about that product is shown (name, description, image, etc.). At the
  bottom the page, users can see more products from the same category.

- The website has a navigation bar that includes the name of the store
  and a link to the home page.

- On the home page, users can change the sorting order. They can sort by
  creation date (new to old, old to new), price (low to high, high to
  low), and alphabetically by name (a to z, z to a). Users can also
  filter products by availability.

- On the category page, user can sort and filter as on the home page.

- Users can search for products whose name matches a given query. Search
  results can be sorted and filtered as on the home page, and further
  filtered by category (i.e., only show products matching the search
  query and in the selected categories). The current search query is
  shown on the results page.

- The logic for sorting, filtering and searching is thoroughly tested
  using Django's testing framework. Be sure to test how different
  criteria interact with one another.
