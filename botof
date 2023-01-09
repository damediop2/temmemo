<?php

if ($_SERVER['REQUEST_METHOD'] === 'POST') {
  // Get the form data
  $name = $_POST['name'];
  $email = $_POST['email'];
  $subject = $_POST['subject'];
  $message = $_POST['message'];

  // Set the recipient email address
  $to = "damealorica@gmail.com";

  // Set the email subject
  $subject = "New contact form submission: $subject";

  // Build the email content
  $email_content = "Name: $name\n";
  $email_content .= "Email: $email\n\n";
  $email_content .= "Message:\n$message\n";

  // Build the email headers
  $email_headers = "From: $name <$email>";

  // Send the email
  mail($to, $subject, $email_content, $email_headers);

  // Redirect to the thank you page
  header('Location: /thank-you.html');
}

?>
