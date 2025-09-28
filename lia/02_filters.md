# Checkpoint 2: Filters

> Due: October 16

> [!IMPORTANT]
> Don't forget to complete your [peer assessment] for the previous
> checkpoint.

Checkpoint 2 focuses on adding searching, sorting and filtering forms to
your views. Here are the requirements:

- Percentage discounts can be applied to products from the admin panel.
  When a product is discounted, users see the new price, the discount
  percentage, and the original price struck through.
- Throughout the website, recently added products are tagged as "new
  arrivals".
- On the home page, users can change the sorting order. They can sort by
  creation date (new to old, old to new), price (low to high, high to
  low), discount percentage (high to low) and alphabetically by name (a
  to z, z to a). Users can also filter products by availability,
  discount and new arrival. More than one filter can be applied at a
  time.
- On the category page, user can sort and filter as on the home page.
- Users can search for products whose name matches a given query. Search
  results can be sorted and filtered as on the home page, and further
  filtered by category (i.e., only show products matching the search
  query and in the selected categories). The current search query is
  shown on the results page.
- The logic for sorting, filtering and searching is thoroughly tested
  using Django's testing framework. Be sure to test how different
  criteria interact with one another.
- Every time changes are pushed to GitHub, your tests are run
  automatically and your code is linted with Ruff.

[peer assessment]: https://forms.gle/K9o9yWipLvBTr6s86
