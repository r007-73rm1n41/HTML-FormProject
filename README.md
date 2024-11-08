# HTML Appointment Form Project 

## Table of Contents
- [Description](#description)
- [Usage](#usage)
- [Form Fields](#form-fields)
- [Code Explanation](#code-explanation)
- [Contribution](#contribution)
- [License](#license)

## Description
The "Appointment Form" project is a simple HTML form designed to facilitate appointment booking for patients to meet doctors for treatment. It collects user details such as name, gender, contact information, appointment date and time, and more. This form is structured using basic HTML form elements to ensure ease of input and submission.

## Usage
To use this form, open the HTML file in any web browser. Patients can enter their details to book an appointment, including name, gender, email, phone number, appointment date, time, and more.

### Steps to Use:
1. Open the HTML file in a browser.
2. Fill out the form fields with appropriate data.
3. Click the "Book Appointment" button to submit the form.

## Form Fields
- **Gender (Radio Button)**
  - Male
  - Female
- **Name (Text Input)**
  - Enter the full name.
- **Email (Email Input)**
  - Enter a valid email address.
- **Phone (Telephone Input)**
  - Enter a 10-digit phone number.
- **Message (Textarea)**
  - Enter any message if needed.
- **Photo (File Input)**
  - Upload an image if applicable.
- **Country (Dropdown Select)**
  - Select a country from the available options.
- **Appointment Date (Date Input)**
  - Select the date for the appointment.
- **Appointment Time (Time Input)**
  - Select the preferred time for the appointment.

## Code Explanation
The form is enclosed within an HTML `<form>` element with the `POST` method. It consists of the following key components:

- **Gender Selection**: Radio buttons for male and female options.
- **Name, Email, and Phone**: Input fields for collecting personal details.
- **Message Textarea**: Allows users to leave an additional message.
- **Photo Upload**: Provides an option to upload a photo.
- **Country Selection**: Dropdown menu for country selection.
- **Appointment Date and Time**: Inputs for specifying the appointment's date and time.

### Example Code Structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Appointment Form</title>
</head>
<body>
    <fieldset>
        <legend>Appointment Form</legend>
        <form method="POST" action="">

            <!-- Gender Selection -->
            <label>Gender</label><br>
            <input type="radio" value="male" name="gender" required /> Male 
            <input type="radio" value="female" name="gender" required /> Female
            <br><br>

            <!-- Name Input -->
            <label>Name</label><br>
            <input type="text" pattern="[a-zA-Z]{3,40}" placeholder="Enter Your Name" name="uname" required />
            <br><br>

            <!-- Email Input -->
            <label>Email</label><br>
            <input type="email" placeholder="Enter Your Email" name="uemail" required />
            <br><br>

            <!-- Phone Input -->
            <label>Phone</label><br>
            <input type="tel" pattern="[0-9]{10}" title="Enter a valid phone number with 10 digits" placeholder="Enter Your Phone" name="uphone" required />
            <br><br>

            <!-- Message Textarea -->
            <label>Message</label><br>
            <textarea name="message" placeholder="Enter Your Message"></textarea>
            <br><br>

            <!-- Photo Input -->
            <label>Photo</label><br>
            <input type="file" name="photo" />
            <br><br>

            <!-- Country Selection -->
            <label>Country</label><br>
            <select name="country" required>
                <option value="">----Select Country----</option>
                <option value="India">India</option>
                <option value="Aus">Australia</option>
                <option value="USA">USA</option>
                <option value="UK">UK</option>
                <option value="Canada">Canada</option>
            </select>
            <br><br>

            <!-- Date Input -->
            <label>Appointment Date</label><br>
            <input type="date" name="appointment_date" required />
            <br><br>

            <!-- Time Input -->
            <label>Appointment Time</label><br>
            <input type="time" name="appointment_time" required />
            <br><br>

            <!-- Submit Button -->
            <button type="submit">Book Appointment</button>
           <!-- <input type="submit" value="Submit" /> -->

        </form>
    </fieldset>
</body>
</html>
```

## Contribution
If you wish to contribute to this project, feel free to:
- Fork the repository.
- Create a new branch (`git checkout -b feature-branch`).
- Commit your changes (`git commit -m "Description of changes"`).
- Push to the branch (`git push origin feature-branch`).
- Create a pull request for review.

## License
This project is open-source and available under the [My_License] license.
