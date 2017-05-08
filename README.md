# JavaScript Playground


Write a JavaScript program to display the current day and time in the following format. Go to the editor
Sample Output : Today is : Friday. 
Current time is : 4 PM : 50 : 22

Solution:

	<script>
    var today = new Date();
    var day = today.getDay();

    var hour = today.getHours();
    var minute = today.getMinutes();
    var second = today.getSeconds();


          switch (day) {
            case 0:
                day = "Sunday";
                break;
            case 1:
                day = "Monday";
                break;
            case 2:
                day = "Tuesday";
                break;
            case 3:
                day = "Wednesday";
                break;
            case 4:
                day = "Thursday";
                break;
            case 5:
                day = "Friday";
                break;
            case 6:
                day = "Saturday";
          }

          var amOrPm = [];

          if (hour>=12 ) {
            amOrPm = 'PM';
          }
          else {
            amOrPm = 'AM';
          }


          document.write("Today is: " + day + "<br>" + "Current time is: " +  hour +  amOrPm + " : " + hour + " : " +  minute);

    </script> 

