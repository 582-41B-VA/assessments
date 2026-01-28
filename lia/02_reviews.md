# Milestone 2: Reviews

> Due: February 11

Milestone 2 focuses on allowing users to review products. Here are the
requirements:

- Users can review products. Each review includes the email of the user,
  a body, and a rating out of 5. The date the review was created is also
  automatically stored and displayed. Users can only leave one review
  per product (i.e., no two reviews can have the same email). The
  average rating of a product is shown on its detail page.

- Users can sort products by their rating (highest to lowest).

- Users can vote a review as "helpful". To do so, they must provide
  their email address. Users can vote on a specific review only once,
  and cannot vote on their own review (i.e., no two votes can have the
  same email, and a vote's email cannot match the review's email). The
  total number of votes is displayed on the review.

- On the product's page, reviews are sorted from most to least helpful.

- Users can flag reviews as "off-topic", "inappropriate" or "fake". Each
  flag includes the email of its author. Users can flag a specific
  review only once. If a review has been flagged more than 5 times, it
  is hidden by default and excluded from the product's average rating.

- Users can add comments on reviews. Each comment includes a body as
  well as the email of its author. The date the comment was created is
  also automatically stored and displayed. Comments are shown in a
  drawer below the review, sorted from newest to oldest.

- Reviews, votes, flags and comments can be viewed and edited from the
  admin panel.

Note that for accessibility reasons your website should remain
functional without JavaScript. Your are also not allowed to use Django's
authentication system yet.

[peer assessment]: https://forms.gle/Hsrsqfn1hTM9Bruf9
