## pseudocode for map and reduce to get null pointer exception count in a log file

map(k=line number, v = line){
    if v contains "NullPointerException" 
        then emit ("NullPointerException",1)
}

Reduce(k , list<v> values){
    int nullPointerExceptionCount =0
    for v in values
        nullPointerExceptionCount = nullPointerExceptionCount + v
    emit ("NullPointerException", nullPointerExceptionCount)
}

######################################### instructions #########################################

github link : https://github.com/shanikaprasangika/EMRNullPointerException

## step 01: create application for null pointer exception count in a log file and create executable jar file

* root directory -> info -> download "create executable jar.pdf" and refer it. finally, you fill get jar
* I added jar file, and you can see it in the following location

    root directory -> info -> EMRNullPointerException.jar

## step 02: run application on AWS EMR 

* root directory -> info -> download "Run application on AWS EMR.pdf" and refer it. finally, you fill get "output" file in AWS S3 location

i attached sample output folder for your reference

   root directory -> info -> output







 
