# ExifJSON
Take a directory of images extract metadata and generate a JSON file with gps coordinates of all images if exists
firts intall package using npm install
then create a directory inside the root directory of the projet
put images files inside that directory
run node index.js ./dir where dir is the name of the directory created before
the script will create a json file called exifdataFile.json containing gps info for each images
a georeferenced directory is created containing only images that have gps coordinates in their exif metadatas
