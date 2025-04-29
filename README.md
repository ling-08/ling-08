<!DOCTYPE html>
<html lang="en">
<head>
   <meta charset="UTF-8">
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Beauty Booking Website</title>

   <!-- Importing Poppins font from Google Fonts -->
   <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

   <style>
      body {
         margin: 0;
         padding: 0;
         height: 100vh;
         background-image: url('bckg.png'); /* Replace with your background image */
         background-size: cover;
         background-position: center;
         background-repeat: no-repeat;
         display: flex;
         justify-content: center;
         align-items: center;
         font-family: 'Poppins', sans-serif;
         overflow: hidden;
         position: relative;
      }

      .container {
         text-align: center;
         background-color: rgba(0, 86, 179, 0.7); /* Blue background with some transparency */
         padding: 40px 50px;
         border-radius: 20px;
         box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
         width: 80%;
         max-width: 650px;
         z-index: 1;
      }

      h1 {
         font-size: 48px;
         font-family: 'Playfair Display', serif;
         font-weight: 700;
         letter-spacing: 1px;
         margin-bottom: 20px;
         color: white;
         text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
         transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
      }

      h1:hover {
         box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
      }

      .btn {
         display: inline-block;
         text-align: center;
         padding: 15px 30px;
         margin: 15px 10px;
         background-color: rgba(0, 86, 179, 0.9);
         color: #fff;
         text-decoration: none;
         font-size: 18px;
         font-weight: 600;
         border-radius: 50px;
         border: 2px solid transparent;
         transition: all 0.3s ease-in-out;
         box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
      }

      .btn:hover {
         background-color: #003d80;
         color: blue;
         transform: translateY(-5px);
         box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
      }

      .icons {
         position: absolute;
         bottom: 30px;
         left: 50%;
         transform: translateX(-50%);
         z-index: 0;
         display: flex;
         gap: 30px; /* Space between the icons */
      }

      .icon {
         width: 50px;
         height: 50px;
         background-color: #fff;
         border-radius: 50%;
         display: flex;
         justify-content: center;
         align-items: center;
         box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
         transition: all 0.3s ease;
         cursor: pointer;
      }

      .icon:hover {
         transform: translateY(-5px);
         box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
      }

      /* Facebook Icon */
      .icon-facebook::before {
         content: "f";
         font-family: 'Poppins', sans-serif;
         font-size: 30px;
         font-weight: bold;
         color: #3b5998; /* Facebook color */
      }

      /* Gmail Icon */
      .icon-gmail::before {
         content: "@";
         font-family: 'Poppins', sans-serif;
         font-size: 30px;
         font-weight: bold;
         color: #d14836; /* Gmail color */
      }

      /* Phone Icon */
      .icon-phone::before {
         content: "📞";
         font-size: 30px;
         color: #34b7f1; /* Phone color */
      }

      /* Hover effect for icons */
      .icon:hover {
         background-color: #f7f7f7; /* Light gray on hover */
      }

      @media (max-width: 768px) {
         h1 {
            font-size: 36px;
         }
         .btn {
            font-size: 16px;
            padding: 12px 25px;
         }
      }

      @media (max-width: 480px) {
         h1 {
            font-size: 28px;
         }
         .btn {
            font-size: 14px;
            padding: 10px 20px;
         }
      }
   </style>
</head>
<body>

   <!-- Main container for content -->
   <div class="container">
      <h1>Welcome to Aruana's Salon</h1>
      <a href="login_form.php" class="btn">Login</a>
      <a href="register_form.php" class="btn">Register</a>
   </div>

   <!-- Custom icons outside the padding area -->
   <div class="icons">
      <!-- Facebook Icon -->
      <a href="https://www.facebook.com/share/1HJko63a39/" target="_blank" class="icon icon-facebook"></a>
      <!-- Gmail Icon -->
      <a href="mailto:daisyjoyarnado@gmail.com" class="icon icon-gmail"></a>
      <!-- Phone Icon -->
      <a href="tel:+639104484678" class="icon icon-phone"></a>
   </div>

</body>
</html>
