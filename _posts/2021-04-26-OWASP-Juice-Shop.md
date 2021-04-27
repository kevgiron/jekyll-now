---
published: false
---


## Week 13 Lab: OWASP Juice Shop

<dl>
  <dt>Task 1</dt>
  <dd>OWASP's, Juice Shop</dd>
 
  <dt>Task 2</dt>
  <dd>What's the Administrator's email address?</dd>
  <dd> admin@juice-sh.op</dd>
  <dt>Task 3</dt>
  <dd> Log into the administrator account</dd>
 
  <dd>Log into the Bender account</dd>
  <dd>Capture the login request </dd>
 
  <dd>fb364762a3c102b2db932069c0e6b78e738d4066</dd>

  <dt>Task 4</dt>
  <dd>Bruteforce the Administrator account's password</dd>
 
  <dd>Once completed, login to the account with the password.</dd>
 
  <dd>c2110d06dc6f81c67cd8099ff0ba601241f1ac0e</dd>

  <dd>Reset Jim's password</dd>
 
  <dd>Inputting that into the Forgot Password page allows you to successfully change his password.</dd>

  <dd>094fbc9b48e525150ba97d05b942bbf114987257</dd>
  
  <dt>Task 5</dt>
  
  <dd>Access the Confidential Documen</dd>

  <dd>We will download the acquisitions.md and save it. After downloading it, navigate to the home page to receive the flag</dd>
 
  <dd>edf9281222395a1c5fee9b89e32175f1ccf50c5b.</dd>
  dd>The password to the mc.safesearch@juice-sh.op account is "Mr. N00dles"</dd>
 
  <dd>66bdcffad9e698fd534003fbb3cc7e2b7b55d7f0</dd>
    <dd> By placing a NULL character in the string at a certain byte, the string will tell the server to terminate at that point, nulling the rest of the string</dd>
 
  <dd>bfc1e6b4a16579e85e06fee4c36ff8c02fb13795</dd>
  
 <dt>Task 6</dt>
 
 <dd>Access the administration page!</dd>
 
  <dd>we need to be in the Admin account in order to view it</dd>
 
  <dd>946a799363226a24822008503f5d1324536629a0</dd>

  <dd>Show the basket of UserID 2</dd>
  <dd>41b997a36cc33fbe4f0ba018474e19ae5ce52121</dd>
  
  <dt>Task 7</dt>
  <dd>Perform a DOM XSS</dd>
 
  <dd>Websites that allow the user to modify the iframe or other DOM elements will most likely be vulnerable to XSS.</dd>

  <dd>9aaf4bbea5c30d00a1f5bbcfce4db6d4b0efe0bf</dd>
  
  <dd>Perform a persistent XSS</dd>

  <dd>Make sure that Burp intercept is on, so it will catch the logout request.</dd>
 
  <dd>The True-Client-IP  header is similar to the X-Forwarded-For header, both tell the server or proxy what the IP of the client is. Due to there being no sanitation in the header we are able to perform an XSS attack.</dd>

  <dd>149aa8ce13d7a4a8a931472308e269c94dc5f156</dd>
  
  <dd>Perform a reflected XSS</dd>
 
  <dd>After submitting the URL, refresh the page and you will then get an alert saying XSS</dd>
 
  <dd>The server will have a lookup table or database </dd>

  <dd>the 'id' parameter is not sanitised before it is sent to the server, we are able to perform an XSS attack. </dd>
  <dd>23cefee1527bde039295b2616eeb29e1edc660a0</dd>
  
  <dt>Task 8</dt>
  <dd>Access the /#/score-board/ page</dd>
 
  <dd>check out the /#/score-board/ section on Juice-shop</dd>

  <dd>7efd3174f9dd5baa03a7882027f2824d2f72d86e</dd>
  
  
 
</dl>
