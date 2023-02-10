# laravel-breeze-web-guard-user-email-otp
Laravel  Breeze Multi-Auth using Web guard

Server Requirements
=====================================
<ul>
  <li>PHP Version => 7.4</li>
  <li>Laravel Version => 8</li>
  <li>MySQl => 5.7+</li>
</ul>

Setup Basic Commands
=====================================
1) git clone repository_url
2) cd laravel-breeze-web-guard-user-email-otp
3) composer update
4) create database and configure .env database connection
5) php artisan migrate
6) php artisan db:seed
7) php artisan serve

Routes Lists
=====================================
<ol>
  <li> Auth Routes </li>
  <ul>
    <li>User Login : http://127.0.0.1:8000/login </li>
    <li>User Register : http://127.0.0.1:8000/register </li>
    <li>Admin Login : http://127.0.0.1:8000/admin/login </li>
    <li>Admin Register : http://127.0.0.1:8000/admin/register </li>
  </ul>
</ol>

Credentials Details
=====================================
<b>User Role</b>
<ul>
  <li>Username : <a href="mailto:user@yopmail.com">user@yopmail.com</a></li>
  <li>Password : user@123456</li>
</ul>

<b>Admin Role</b>
<ul>
  <li>Username : <a href="mailto:admin@yopmail.com">admin@yopmail.com</a></li>
  <li>Password : admin@123456</li>
</ul>

Project Requirement 
=====================================
<ol>
  <li> Authentication Using Laravel Web Gaurd : </li>
  <li>Admin Role Requirement </li>
    <ul>
      <li> <b> Admin Registration Fields </b> </li>
      <li> Name : [ Validation Rules : Accept only strings and space, Required ] </li>
      <li> Email : [ Validation Rules : Accept only valid email address, Required ] </li>
      <li> Password : [ Validation Rules : Accept only valid password min 8 length with alphanumeric, Required ] </li>
      <li> Confirm Password : [ Validation Rules : should be same as Password field, Required ] </li>
      <li> On Registration button click redirect to Admin dashboard page </li>
      <li> Use migrations scrpits for tables </li>
      <li> Generate 5 dummy sample for Admin role using Factory and Seeder </li>
      <li> Follow PHP/Laravel code standards </li>
      <li> Make Seprate dashboard view ,admin table and Admin model </li>
      <li> <b> Admin Login Fields </b> </li>
      <li> Email : [ Validation Rules : Accept only valid email address, Required ] </li>
      <li> Password : [ Validation Rules : Accept only valid password min 8 length with alphanumeric, Required ] </li>
      <li> On Login button click redirect to Admin dashboard page if credential is validated </li>
    </ul>
  <li>User Role Requirement</li>
      <ul>
          <li> <b> User Registration Fields </b> </li>
          <li> Name : [ Validation Rules : Accept only strings and space, Required ] </li>
          <li> Email : [ Validation Rules : Accept only valid email address, Required ] </li>
          <li> Password : [ Validation Rules : Accept only valid password minimum 8 length with alphanumeric, Required ] </li>
          <li> Confirm Password : [ Validation Rules : should be same as Password field, Required ] </li>
          <li> On Registration button click send email verification 8 digit OTP to registered email address </li>
          <li> Verify OTP Page will be open with Enter OTP </li>
          <li> 1 minutes timer counter will shows to user </li>
          <li> After 1 minutes timer counter will shows Resend OTP button to user and should able to resend 8 digit OTP at registered email</li>
          <li> After 1 minutes timer counter old OTP will be expired and not allow to login with old OTP</li>
          <li> On Verify OTP Check if OTP is valid then redirect to User Home Page </li>          
          <li> Use migrations scrpits for tables </li>
          <li> Generate 5 dummy sample for User role using Factory and Seeder </li>
          <li> Follow PHP/Laravel code standards </li>
          <li> Make Seprate dashboard view ,user table and User model </li>
          <li> <b> User Login Fields </b> </li>
          <li> Email : [ Validation Rules : Accept only valid email address, Required ] </li>
          <li> Password : [ Validation Rules : Accept only valid password min 8 length with alphanumeric, Required ] </li>
          <li> On Login button click redirect to User home page if credential is validated </li>
      </ul>
</ol>
  
References : 
=====================================
a) https://www.youtube.com/watch?v=yXjHYTFRTC8

