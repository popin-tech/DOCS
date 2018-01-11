# USER AUTHENTICATION

### FRONT-END

* User should be able to sign in and sign up with Facebook.
* User should be able to sign in and sign up with Google.
* User should be able to sign in and sign up with Instagram.
* When a user signs in or signs up, and they haven’t got a role, they should be redirected to the ‘Get Started’ page.
* When user is already in the database but signs up they should be directed to their profile page.

### BACKEND

* Create a process to allow for user creation or authentication , which result in a token being sent.

# BRAND JOURNEY

### FRONT-END

* Brand should see an explainer.
* A: User should add their brand name
* A: User should describe themselves
* B: User should choose up to three categories.
* B: User should pick their ideal customer, up to three choices
* C: User should be able to add their products.
* When User finishes their brand on-boarding they should see a congratulations page.

### BACKEND

* Create a Brand with a user attached and add to the database.

# SPACE JOURNEY

### FRONT-END
* Space should see an explainer
* A: User should add their space name
* A: User should be able to enter location and choose and address from drop down
    * Use google places api to look up address
* B: User should pick what kind of demographic their space caters for
* B: User should pick what kind of category of brands they are best for
* C: User should be able to book a photo appointment by first picking a day.
* C: User should be able to book a photo appointment by secondly pick a time.

### BACKEND

* Create a Space with a user attached and add to the database.
* Get available appointments.
* Create an appointment date and notify vettors.

# SPACE PROFILE PAGE
### FRONT
* A Space should see their profile page on ‘un-publish mode’ when they first sign up
  * See wireframes
* After Space has been approved they should be able to see their profile in ‘publish mode’
  * See wireframe

### BACKEND
* Update Space object 'approved' field to either true or false
  * default is false
  * After vetting, when a space has been approved, 'approved' need to changed to true.

# SPACE ADDING ADDITIONAL AREAS

* Space should be able to add additional space
  * See wireframe for journey

### BACKEND
* Update Space object with new AREAS
    * AREA field 'approved' will be set to false as default
    * After vetting, 'approved' status changes accordingly
* Create an appointment date and notify vettors.   
    * Appointment 'status' starts off as Pending

# SPACE BOOKINGS PAGE

### FRONT END
* Space should be able to see all their bookings when they go their booking page
* There should be three tabs
  * Pending
  * Accepted
  * Cancelled
* They should first see the Pending bookings tab.
  * See wireframes
* On the Pending tab, Space should be able to see a ‘new’ button on bookings and read status 'unseen'
* When the pending booking has been opened by the Space the read status should change to ‘seen’
* Space should ONLY SEE the 'add card button' instead of card details, when they HAVE NOT added a card before. __first time__
* When a Space has a card they should see 'pick another card' or 'add a new card' button.
* Space should be able to add a new card by being directed to the ‘add new card’ page.
* Space should be able to pick a new card by being directed to the ‘pick a new page’
* Space should be able to change bookings to auto accept.
* This would result in a new booking status automatically being ‘accepted’


## BACK END
* Update read status for Space
* This makes a post (new)/ patch (additional) request that updates the spaces cards field.
*This should result in the card picked becoming default.
* This should result in a new card being added
* The newly added card should than become default

#### SPACE ACCEPTING A BOOKING

## FRONT END

 * Space should only be allowed to accept booking when a card is added

## BACKEND

* When a Space accepts a booking it should change the booking status to ‘accepted’
* When a Space accepts a booking is should change read status for Brand to 'unseen'.
* When a Space accepts a booking, payment will be made to the Space’s card.

#### SPACE CANCELLING A BOOKING

## BACKEND

* When a Space rejects booking it should change booking status to 'cancelled'.
* When a Space rejects a booking it should change read status for Brand to 'unseen'.

## BRAND PROFILE PAGE

* A Brand should see their profile page on ‘un-publish mode’ when they first sign up
* After Brand has been finished completing the step remaining they should be able to see their profile in ‘publish mode’
  * See wireframe

## BRAND BOOKING SPACE

* Brand should be able to see all space available when they go to the ‘find a space’ page.
* When Brand clicks on space profile, they should be see the Space profile in ‘public’ mode.
* When brand clicks on the availability of  a space this should take them to the area show page
* The Brand should be able to see available dates, unavailable time should be disabled.
* Brand should be able to pick one or more dates for their booking.
* When a Brand request a booking , this should take them to the booking confirmations page.
* If it’s the first time a Brand is requesting a booking they should see the Add a card button only.
* If it’s not the first time a Brand is requesting a booking they should be able to either add a new card or pick a card.
* When a Brand adds a new card this card should become default.
* When a Brand picks a new card this card should become default.
* Brand should than be able to confirm the the booking request.
* When a Brand confirms a booking this should create a new booking with a status of ‘pending’
* When a Brand confirms a booking this should result in the booking payment amount  being ring fenced.
* When a Space accepts a booking the payment from the Brand is then taken.

## BRAND BOOKINGS PAGE

* Brand should be able to see all their bookings when they go their booking page
* There should be three tabs
  * Pending
  * Accepted
  * Cancelled
* They should first see the ‘Accepted’ bookings tab.
  * See wireframes
* Brand should be able to cancel booking before cancellation period has finished.
* Brand should be able to add to calendar their booking dates.
* When accepted or cancelled booking is not seen yet, it should have a status of ‘unseen’, this will result in a new button being added to the booking heading.
* When a accepted or cancelled booking is seen the status of the booking should change to ‘seen’.


## MESSAGING

* When brand or space click on the messaging icon on each other pages, this should taken them to their chat page.
* If it’s the first time both of the brand or space are messaging each other , a new chat should be created.
* If it’s not the first time both of the brand or space are messaging each other, this action should take them to their existing chat.
* When message first sent , it should have the status of ‘unseen’
* When a message is seen by Brand or Space it should then have a status of ‘seen’
* When there is unseen messages it should show on the Brand or Space Chat icons
* The message that is previewed is the last sent message in the Chat.

## USER SETTINGS

* Space and brand can access their user setting when they click on the avatar icon and click on the settings link.
* Users can edit their Personal details.
* User should be able to connect or discount to a social account.
* User should be able to deactivate their account
* Users should be able to delete their account

## LOG OUT

* Users should be able to log out by clicking on their icon and click on the logout button
* This should result in the token being removed from the browser.
* The user should than be redirected to the landing page.

## PROFILE Status
 * publish: TRUE
          : FALSE

## APPOINTMENT STATUSES

* Pending
* Attended
* Completed


## AREA STATUS

* Approved : TRUE
           : FALSE


## Booking
    * Status (As Constants)
        * Pending
        * Accepted
        * Cancelled
    * brandReadStatus
        * 'seen' / 'unseen'   
    * spaceReadStatus
        * 'seen' / 'unseen'
