# DESAFIO-QA-BEEDOO
Project related to Beedoo's Junior Software Quality Analyst challenge.

## 1. Test Scenarios in Gherkin
All test scenarios relating to the challenge are concentrated in the following document:
https://docs.google.com/spreadsheets/d/1SzYEjzOqDCW8_rgwmWl07xbzS1guHYp4/edit?usp=drive_link&ouid=108401444136857796415&rtpof=true&sd=true


##  2. Bugs Found

2.1. End Date Accepting Value Less Than Start Date
Description: The end date field accepts a value that is earlier than the start date.

Steps to Reproduce:
Go to the course creation page.
Enter a start date.
Enter an end date that is earlier than the start date.
Click the "Register Course" button.

Expected Result: The system should display an error message.

Actual Result: The course is registered despite the invalid dates.

2.2. Unable to Delete Course Despite Success Message
Description: The course is not removed from the list even though a success message is shown.

Steps to Reproduce:
Go to the course list page.
Click "Delete" next to a course.
Confirm the deletion.
Observe the success message.

Expected Result: The course should be removed from the list.

Actual Result: The course remains in the list.

2.3. Course Name Accepting More Than 255 Characters
Description: The "Course Name" field allows more than 255 characters.

Steps to Reproduce:
Go to the course creation page.
Enter a course name with more than 255 characters.
Click "Register Course".

Expected Result: The system should restrict the name to 255 characters.

Actual Result: The course is registered with a long name.

2.4. Allows Creating Course with Blank Fields
Description: The system allows creating a course with all fields blank.

Steps to Reproduce:
Go to the course creation page.
Leave all fields blank.
Click "Register Course".

Expected Result: The system should prompt to fill in mandatory fields.

Actual Result: The course is created with blank fields.

2.5. Number of Vacancies Accepting Negative Values
Description: The "Number of Vacancies" field accepts negative values.

Steps to Reproduce:
Go to the course creation page.
Enter a negative value in the "Number of Vacancies" field.
Click "Register Course".

Expected Result: The system should display an error for negative values.

Actual Result: The course is registered with negative vacancies.

2.6. Layout Misconfiguration
Description: Layout issues on the course creation page, such as misaligned or overlapping elements.

Steps to Reproduce:
Go to the course creation page.
Observe the layout.

Expected Result: The layout should be clean and properly aligned.

Actual Result: The layout is misconfigured.

Evidences: https://drive.google.com/file/d/1nYpWS7lEthTExxrlz_aoYZZ9YRgpVy5T/view?usp=drive_link


## 3. Proposed Improvements

3.1. Add Cancel Button in Course Creation Form

Description: Add a "Cancel" button to allow users to discard changes and exit the course creation process.

Benefits: Provides users with a way to exit the form without saving incomplete data.

3.2. Add Sorting Options to Course List

Description: Implement sorting options (by name, date, instructor) in the course list.

Benefits: Enhances usability by allowing users to organize courses according to different criteria.

3.3. Limit Character Count to Prevent Layout Issues

Description: Set maximum character limits for fields to avoid layout distortion.

Benefits: Ensures a consistent and visually appealing layout.

3.4. Define and Enforce Mandatory Fields for Course Creation

Description: Specify which fields are mandatory and prevent course creation if these fields are not filled.

Benefits: Ensures that all required information is provided before course registration.

Evidences: https://drive.google.com/file/d/1_FhaR9aNR4bfuGQaypEcmEa-g6bSm-Ne/view?usp=drive_link
