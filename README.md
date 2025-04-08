# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Meta information and title for the page -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Form</title>
</head>
<body>

    <!-- Header Section -->
    <header>
        <h1>Registration Form</h1>
        <p>Please fill out the form to register.</p>
    </header>

    <!-- Main Content Section -->
    <main>
        <!-- Registration Form -->
        <form action="/submit" method="POST">
            <!-- Name Field -->
            <section>
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>
            </section>

            <!-- Email Field -->
            <section>
                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email" required>
            </section>

            <!-- Password Field -->
            <section>
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" placeholder="Enter a strong password" required minlength="8">
            </section>

            <!-- Date Field -->
            <section>
                <label for="dob">Date of Birth:</label>
                <input type="date" id="dob" name="dob" required>
            </section>

            <!-- Dropdown (Select) -->
            <section>
                <label for="country">Country:</label>
                <select id="country" name="country" required>
                    <option value="">Select your country</option>
                    <option value="usa">United States</option>
                    <option value="canada">Canada</option>
                    <option value="uk">United Kingdom</option>
                    <option value="aus">Australia</option>
                </select>
            </section>

            <!-- Radio Buttons (Gender) -->
            <section>
                <fieldset>
                    <legend>Gender:</legend>
                    <label for="male">
                        <input type="radio" id="male" name="gender" value="male" required> Male
                    </label>
                    <label for="female">
                        <input type="radio" id="female" name="gender" value="female"> Female
                    </label>
                    <label for="other">
                        <input type="radio" id="other" name="gender" value="other"> Other
                    </label>
                </fieldset>
            </section>

            <!-- Checkboxes (Interests) -->
            <section>
                <fieldset>
                    <legend>Interests:</legend>
                    <label for="sports">
                        <input type="checkbox" id="sports" name="interests" value="sports"> Sports
                    </label>
                    <label for="music">
                        <input type="checkbox" id="music" name="interests" value="music"> Music
                    </label>
                    <label for="travel">
                        <input type="checkbox" id="travel" name="interests" value="travel"> Travel
                    </label>
                </fieldset>
            </section>

            <!-- Submit Button -->
            <section>
                <button type="submit">Register</button>
            </section>
        </form>
    </main>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 Registration Website</p>
    </footer>

</body>
</html>

Happy Coding! 💻✨
