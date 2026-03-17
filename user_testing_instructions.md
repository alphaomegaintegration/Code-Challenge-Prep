
# User Testing Instructions

## Persona: Student

### Scenario 1 — Student Can Register

**Objective**  
Verify that a new user can successfully register on the C2C platform and log in with the newly created credentials.

**Steps**

1. Navigate to the C2C application.
2. Click **Create Account**.
3. The Student Registration page is displayed.
4. Fill in the registration form.

**Student Information**
- Student First Name: Nancy
- Student Last Name: Drew
- Date of Birth: 06/12/2008
- Student ID Number: 1234
- Student Phone Number: 478-606-4489

**Address Information**
- Street Address: 18 River Heights Drive
- City: River Heights
- State: IL
- Zip Code: 60174

**Parent / Guardian Information**
- Parent First Name: Carson
- Parent Last Name: Drew
- Relationship to Student: Father
- Parent Email Address: carsondrew@gmail.com
- Parent Phone Number: 478-606-4491

**Academic Information**
- Dormitory: Maple Hall
- Academic Level: Sophomore
- Major: Arts

**Login Credentials**
- Email Address: nancydrew@gmail.com
- Password: WhiteBoardMarker13$@
- Confirm Password: WhiteBoardMarker13$@

5. Click **Register**.
6. You will be navigated to the Login page where a **Successful Registration** message appears.

**Expected Result**
- The user account is successfully created on the C2C platform.

---

### Scenario 2 — Log In as Student

**Objective**  
Verify that a user can successfully log into the C2C platform as a student.

**Steps**
1. Enter credentials:
   - Email: nancydrew@gmail.com
   - Password: WhiteBoardMarker13$@
2. Click **Sign In**.

**Expected Result**
- User successfully logs in.
- Student Dashboard appears.

---

### Scenario 3 — Make a Booking

**Objective**  
Verify that a user can search for transportation and complete a booking.

#### Task 1 — Search Flight
1. Click **Search Transportation**
2. Enter:
   - Destination: DCA – Ronald Reagan Washington National Airport
   - Departure Date: 04/21/2026
3. Click **Search Flights**
4. Select the first flight.

#### Task 2 — Search Shuttle
1. Select **Botanical Garden** pickup location.
2. Click **Search Transportation**
3. Review shuttle options.
4. Select the first shuttle option.

#### Task 3 — Confirm and Pay
1. Review itinerary.
2. Add tip: **$2**
3. Choose **Pay with Stripe**
4. Enter card:

```
4242 4242 4242 4242
Exp: 12/27
CVC: 769
Zip: 60174
```

5. Click **Pay**
6. Click **Book Shuttle**

**Expected Result**
- Shuttle booking completed
- Confirmation message appears
- Trip appears in **Upcoming Trips**

---

### Scenario 4 — Access Boarding Pass & Track Shuttle

**Objective**  
Verify student can download boarding pass and track shuttle.

**Steps**
1. Login with test credentials
2. Navigate to **Upcoming Trips**
3. Download **QR Boarding Pass**
4. Click **Where’s My Shuttle**

**Expected Result**
- Boarding pass downloads
- Map displays shuttle location and ETA

---

### Scenario 5 — Rate Completed Trip

**Objective**  
Verify students can rate completed rides.

**Steps**
1. Login as student
2. Click **Rate Your Experience**
3. Select **5 stars**
4. Enter feedback:

```
Amazing experience. The driver was very courteous. Reached airport on time.
```

5. Click **Submit**

**Expected Result**
- Rating saved
- Rating option becomes inactive

---

## Persona: Administrator

### Scenario 1 — View Dashboard Metrics

**Objective**  
Verify administrator login and dashboard visibility.

**Expected Result**
Administrator can view:
- Demand Forecasting stats
- Occupancy & Sales stats
- Admin management links

---

### Scenario 2 — View and Manage Bookings

Administrator can:
- View booking list
- Open booking details
- Change pickup location
- Cancel booking
- View cancelled booking status

---

### Scenario 3 — Manage Shuttle Path

Administrator can:
- Edit shuttle routes
- Notify passengers
- Override seats
- Cancel shuttle
- Configure stops

---

### Scenario 4 — Respond to Ratings

Administrator can:
- View ratings
- Read feedback
- Click **Respond**
- Open email via mailto link

---

### Scenario 5 — Manage Student Registration

Administrator can:
- View registration details
- Toggle **Financial Aid Eligible**
- Update parent phone number
- Save record

---

## Persona: Operator

### Scenario 1 — View Passenger Manifest

**Objective**  
Verify operator can access passenger manifest.

**Steps**
1. Login as Operator
2. View upcoming trips
3. Click **View Passenger Log**

**Expected Result**
Passenger manifest displays:
- Student Name
- Pickup Stop
- Trip details
