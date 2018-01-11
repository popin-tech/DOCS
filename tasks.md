# USER AUTHENTICATION

FRONT-END

* User should be able to sign in and sign up with Facebook.
* User should be able to sign in and sign up with Google.
* User should be able to sign in and sign up with Instagram.
* When a user signs in or signs up, and they haven’t got a role, they should be redirected to the ‘Get Started’ page.
* When user is already in the database but signs up they should be directed to their profile page.

BACKEND

* Create a process to allow for user creation or authentication , which result in a token being sent.

# BRAND JOURNEY

FRONT-END

* Brand should see an explainer.
* A: User should add their brand name
* A: User should describe themselves
* B: User should choose up to three categories.
* B: User should pick their ideal customer, up to three choices
  C: User should be able to add their products.
  When User finishes their brand onboarding they should see a congratulations page.
  BACKEND
  Create a Brand with a user attached and add to the database.

# SPACE JOURNEY

FRONT-END

A: User should add their space name
A: User should be able to enter location and choice and address from drop down
Use google places api to look up address
B: User should pick what kind of demographic their space caters
B: User should pick what kind of category of brands they best for
C: User should be able to book a photo appointment by first pick a day.
C: User should be able to book a photo appointment by secondly pick a time.
BACKEND
Create a Space with a user attached and add to the database.

# SPACE PROFILE PAGE

A Space should see their profile page on ‘unpublish mode’ when they first sign up
See wireframes
After Space has been approved they should be able to see their profile in ‘publish mode’
See wireframe

# SPACE ADDING ADDITIONAL AREAS

Space should be able to add additional space
See wireframe for journey

SPACE BOOKINGS PAGE
Space should be able to see all their bookings when they go their booking page
There should be three tabs
Pending
Accepted
Cancelled
They should first see the pending bookings tab.
See wireframes
Space should be able to see the ‘new’ button added to unopened bookings
When the booking has - been opened the mode should change to ‘seen’
Space should see only the add card button when they have not added a card before.
Space should see add another card or pick another card button when they have added a card before.
Space should be able to add a new card by being directed to the ‘add new card’ page
This should result in a new card being added
The newly added card should than become default
Space should be able to pick a new card by being directed to the ‘pick a new page’
This should result in the card picked becoming default.
Space should be able to change bookings to auto accept.
This would result in a new booking status automatically being ‘accepted’
SPACE ACCEPTING A BOOKING
When a Space accepts a booking it should change the booking status to ‘accepted’
Space should only be allowed to accept booking when a card is added
When a Space accepts a booking , payment should added to the Space’s card.
SPACE CANCELLING A BOOKING
When a Space rejects booking it should change booking status to cancelled
