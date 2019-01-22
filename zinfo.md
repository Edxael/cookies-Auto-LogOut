


Cokies
https://www.tutorialspoint.com/javascript/javascript_cookies.htm

https://www.tutorialspoint.com/How-to-set-cookies-to-expire-in-30-minutes-in-JavaScript









<script>

    function WriteCookie() {
      console.log("Running: WriteCookie()")
      var cookieTime = new Date();
      var minutes = 30;

      cookieTime.setTime(cookieTime.getTime() + (minutes * 2 * 1000));
      // cookievalue = escape(document.myform.customer.value) + ";"

      document.cookie = "name=" + "User";
      document.cookie = "expires=" + cookieTime.toUTCString() + ";"

      console.log("Info: ", document.cookie)
      document.write("Setting Cookies : " + "name=" + "Edxael");
    }

    WriteCookie()

    // setInterval(function(){ alert("Hello"); }, 2000)
    setInterval(() => { 
      // alert("Hello"); 
      // let now = Date()



      console.log("The cookie time: ", typeof document.cookie)
      }, 3000)
  
</script>