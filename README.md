## PHP Mailer

```php
include "SMTP.php";
include "PHPMailer.php";
include "Exception.php";

use PHPMailer\PHPMailer\PHPMailer;


$mail = new PHPMailer;
$mail->IsSMTP();
$mail->Host = 'smtp.gmail.com';
$mail->SMTPAuth = true;
$mail->Username = 'your email';
$mail->Password = 'secret';
$mail->SMTPSecure = 'ssl';
$mail->Port = 465;
$mail->setFrom('your email', 'Reset Password');
$mail->addReplyTo('your email', 'Reset Password');
$mail->addAddress($email);
$mail->isHTML(true);
$mail->Subject = '';

$bodyContent = "";

$mail->Body = $bodyContent;
```
