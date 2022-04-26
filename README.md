# ExifJSON
Take a directory of images extract metadata and generate a JSON file with gps coordinates of all images if exists
firts intall package using npm install
then create a directory inside the root directory of the projet
put images files inside that directory
import package in your script using for example using const jsonExif= require ('exif-json') 
run your script and indicate as an argument the directory where images are stored (ex :  node myscript.js ./pics)
if no argument is specified the package will search for a './photos' directory
you can also indicate the directory as an argument of the imported function
(ex jsonExif('./pics')). if so the argument in the function supersedes the argument on the command line
the script will create a json file called exifdataFile.json containing gps info for each images.
the json file present gps coordinates in two ways
    1/ cardinal deg min sec (ex N 45 2 14.5 E 5 38 43.91)
    2/ deg signed with decimal (ie 43.59563 -1.2589652)
the json file also indicate altitude if exits
a  directory called georeferenced is created containing only images that have gps coordinates in their exif metadatas
