# Milestone 4: Accounts

> Due: November 27

Milestone 4 focuses on adding authentication. Here are the requirements:

- Users can register an account by providing their name, email, and
  password. Once the account has been created, they are redirected to a
  login page.

- Users can log in with their email and password. Once they are logged
  in, users are redirected to their account page.

- On the account page, users can change their name, email, and password.
  They can also access a list of their orders. Clicking on an order
  brings them to an order detail page where information about that order
  (products, quantity, date, total) is shown.

- On the login page, users who have forgotten their password can click
  on a link to reset it. To reset their password, users must provide
  their email address. If the address matches an account, a reset link
  is sent that address.

- When a user is authenticated, their cart is stored in the database
  instead of in their session. If their session cart contains items when
  they log in, those items are transferred to their database cart.

- On a product's detail page, authenticated users can add the product to
  their wish list. When they do so, a flash message confirms that the
  action was successful.

- Authenticated users can access their wish list from the website's
  navigation. The wish list page lists products currently in the user's
  wish list. For each product, its name, image and price (incl. discount
  if applicable) are shown. Users can remove products from their wish
  list, or transfer them to their cart. When they do so, a flash message
  confirms that the action was successful.

- Users must now be authenticated to review a product, vote or flag a
  review, and leave a comment. When performing these actions, they no
  longer need to provide their email, as account-based validation is
  used instead. Furthermore, only users who have purchased a product can
  now review that product.

- When authenticated users check out their cart, their name, email and
  address is sent to Stripe so that they don't have to type it again on
  Stripe's hosted checkout page.
