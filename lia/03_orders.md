# Milestone 3: Orders

> Due: February 25

Milestone 3 focuses on allowing users to buy products. Here are the
requirements:

- On a product's detail page, users can add one or more instances of the
  product to their shopping cart. Once they've done so, they are
  redirected to a shopping cart page where a flash message confirms the
  item or items were successfully added.

- The shopping cart page lists products currently in the user's cart.
  For each product, its name, image, unit price , and total price (unit
  × quantity) are shown. The order's total is also displayed.

- Users can remove products from their shopping cart and change the
  quantity to purchase. Once they've done so, a flash message confirms
  that the action was successful. The message includes the name of the
  product and summarizes the change (e.g., "Product A was removed from
  your shopping cart" or "The quantity of Product B was changed from 2
  to 1").

- From the shopping cart page, users can proceed to check out their
  order. The checkout process is handled by Stripe's hosted checkout (as
  seen in class). In addition to payment information, it also collects
  the customer's name, email, and billing and shipping addresses.

- Before users are redirected to Stripe's hosted checkout, their order
  is saved in the database. An order stores the date when it was
  created, the [payment ID] , the name of the customer, their email,
  billing and shipping addresses. The order's items (incl. their price
  when purchased and quantity) are also saved in the database. The
  checkout session's [client reference ID] is set to the order's ID.

- Once users are redirected to the payment success page, their shopping
  cart is emptied.

- Once the checkout has been fulfilled (i.e., when Stripe sends the
  confirmation to your webhook endpoint), the order is updated. The ID
  of the order to update is retrieved from the request's body, which
  includes the [client reference ID] stored previously.

- Orders and the items they contain can be viewed and edited from the
  admin panel.

- The website's header includes a link to the cart. The link's label
  shows how many items are currently in the cart.

[peer assessment]: https://forms.gle/AoNK1f2Cnaa5dpjZ6
[payment ID]: https://docs.stripe.com/api/checkout/sessions/object#checkout_session_object-payment_intent
[client reference ID]: https://docs.stripe.com/api/checkout/sessions/object#checkout_session_object-client_reference_id
