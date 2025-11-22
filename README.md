📧 Google Sheets Automated Email Sender (Daily Feedback Email Script)

This Google Apps Script automatically sends customized feedback request emails from a Google Sheet, logs all activity in a separate sheet, and provides a custom menu to trigger email sending manually.

📌 Features

✔ Sends personalized emails to recipients listed in Google Sheets
✔ Adds a custom "Email Actions" menu in the Google Sheets UI
✔ Creates a separate Email Log sheet automatically to track sent emails
✔ Prevents duplicate sending by marking emails as Sent
✔ Uses HTML formatting for rich and professional email body
✔ Logs both successful and failed emails with timestamp and subject

📄 How It Works

The script reads data from the active sheet.

For each row, it checks:

Recipient Name

Recipient Email

Status (whether the email is already sent)

If the email is not marked Sent, it sends a personalized HTML email.

After sending:

Updates the sheet's Status column to Sent

Logs the activity in the Email Log sheet (auto-generated if it doesn’t exist)

🧾 Data Format (Google Sheet Structure)
Column A	Column B	Column C
Name	Email	Status
John Doe	john@test.com
	leave blank
Jane Doe	jane@test.com
	Sent

Note: The script only sends emails where Status is empty or not equal to "Sent".

🔧 Custom Menu

After adding the script, a new menu will appear in your Sheet:

📌 Email Actions → Send Daily Emails

You can manually trigger the script anytime using this menu option.

📮 Email Content

The script sends a feedback request email with:

Personalized greeting (Dear <Name>)

Company signature & logo

Survey form link

Professional HTML formatting
