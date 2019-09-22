# Cp202Bonus
Description of how the validation code was created and decoded

The verification code was generated through Cookies.js javascript code found when you inspect the validation page of Quiz 1 part 1 (the pink page). The Cookies.js javascript code can be found under the "Sources" tab of the inspect page.

One can decode the the validation string by going to the their local wlu folder that had been cloned from https://github.com/josefelixsandoval/wlu.git

From the wlu folder, go to www > CP202 > Fall2019 > q1validation > check_keys > index.html which will open a page where you can enter the validation string under "Encoded key" box, click on show "Key value", and the decoded key, in my case "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.132 Safari/537.36::h=1050::w=1680::plugin_name=Chrome PDF Plugin::450101465373676038091325373631050168024"

The decoding code of such a validation string can be found when you inspect the encode/decode html page, which, under the "Sources" tab, one can see the Window "atob" method was used to decode a base 64 encoded string 
