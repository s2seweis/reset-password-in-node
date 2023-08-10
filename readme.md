# Secure Password Reset 


## Tutorial Origin: https://blog.logrocket.com/implementing-secure-password-reset-node-js/


### SignUp = http://localhost:8080/api/v1/auth/signup

<!-- {
  "email": "weissenborn.sebastian@gmail.com",
  "name":"s2seweis",
  "password":"law123"
} -->

<!-- result: create user

{
  "userId": "64d49a1b9b1d87292090cb2c",
  "email": "weissenborn.sebastian@gmail.com",
  "name": "s2seweis",
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY0ZDQ5YTFiOWIxZDg3MjkyMDkwY2IyYyIsImlhdCI6MTY5MTY1NDY4M30.wa-8vuhKvHSF5TWIrqMzhttH47NDhUVTj27cOpGzpHM"
} -->

### Request Reset Password = http://localhost:8080/api/v1/auth/requestResetPassword

<!-- {
  "email": "weissenborn.sebastian@gmail.com"
} -->

<!-- result: Response includes a link with a token and the userId

{
  "link": "localhost://8090/passwordReset?token=9431145a68d5f41628f00010b7ec2e2abdca43e2eadf83df7c730eec6e66020a&id=64d49a1b9b1d87292090cb2c"
} -->

### Reset Password = http://localhost:8080/api/v1/auth/resetPassword

<!-- {
  "userId": "64d49a1b9b1d87292090cb2c",
  "token":"9431145a68d5f41628f00010b7ec2e2abdca43e2eadf83df7c730eec6e66020a",
  "password": "law123"
} -->

<!-- Result: Reset of the password

{
  "message": "Password reset was successful"
} -->

### At the moment:

# https://www.youtube.com/watch?v=lBRnLXwjLw0
# https://kinsta.com/blog/gmail-smtp-server/
# http://nodemailer.com/about/

### Sending and Receiving Emails is working



