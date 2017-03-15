# IT102.FINAL.Project1
Objects and methods
The code below defines an object prototype called "car". Car needs to have the following features:

Properties:

    gas (number type)
    mpg (number type)
    range (number type)
    empty (boolean type)

Methods:

    drive(miles) (no return value)
    fill(gallons) (no return value)

Your job is to supply the missing properties and methods. Here are some notes to help you out:

    range = gas * mpg
    fill(gallons) should update both gas and empty

Test code is included below. After you have finished the object prototype, run the script including the test code and verify that the test code runs as expected. Then submit your finished prototype and test code to the dropbox. 

 <!--

------------------------------------- Partially Complete Script ------------------------------

<!DOCTYPE html>
<html>
<body>

<p id="demo"></p>

<script>
function car(gas, mpg) {
this.gas = gas;
if (this.gas <= 0){this.empty = true;}

this.drive = function (miles) {
this.gas -= miles/this.mpg;
if(this.gas <=0) {
this.empty = true;
}
};

this.fill = function (gallons){
};

}

 

//test code

var test = new car(15, 30);
alert (test.empty); //expected output = false
test.drive(500);
alert (test.empty); //expected output = true
test.fill(20);
alert (test.empty); //expected output = false

</script>

</body>
</html>

-->
