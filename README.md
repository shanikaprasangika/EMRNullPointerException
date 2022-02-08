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

## instructions 




 
