## 2FA code machine
There is another version of Google Authenticator, but code is more hard. Sorry if it take your time, but this is my final way.
<br>
## What it can do?
1. Enable 2FA
2. Secure your account by setting password
3. Coded as JavaScript, that you can easiler change the code for more secure (because JavaScript is easy)
4. You can "say" with your web API to create an authenticator code
5. The authenticating key minium length is 12 characters. Key will store as Base64 or Buffer
## Heyy, don't be too hurry
#### Lost your account by losing this authenticator
DO NOT delete this authenticator before turning off 2FA. You cannot apply any hack because the code is very hard and change itself per 25 seconds. <br>
DO NOT sell any gap in this authenticator... but you can sell it because i not have any credit and i just 17 years old 😅
#### Compatible with ALL web APIs
Copy this code to your web:
```html
<script src="https://coldsnow-officalweb.tempfor.repl.co/security/2fa/code/index.js"></script> <!-- GitHub repo: https://github.com/ColdSnow2/2FA-code-machine -->
<input id="2fa">2FA code</input>
<button onclick="compare()">Check your code and pass</button>
<script>
  function compare() {
    const userinput = document.getElementById('2fa').innerText;
    const twof = twofactor.output()
    if(userinput == twof) { // CASE pass
      document.getElementById('your-displayer-id-or-html-element-id-goes-here').innerText = twof // Get 2FA code
      window.location.replace('your-url-goes.here')
    } else { // CASE invalid code or code isn't the code generated by the generator
      document.getElementById('your-display-or-html-element-id-goes-here').innerText = You've enter wrong code
    }
 }
</script>
```
##Thanks for use
ColdSnow2 - Discord: MyCoolestDay123#2436
